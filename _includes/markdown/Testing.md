<h2 id="code-coverage" class="anchor-heading">Code coverage {% include Util/link_anchor anchor="code-coverage" %} {% include Util/top %}</h2>

Every feature should be accompanied by tests and all pull requests should come with associated tests, all living within the `tests` directory.  While we have no intention of striving for 100% code coverage, we should aim for above 80% with above 90% being the ideal.  We should also look to utilize a code coverage / automated code review tool like [Coveralls](https://coveralls.io/), [Code Climate](https://codeclimate.com/), or [Codecov](https://codecov.io/) and ensure that is a pull request requirement before merging.

<!-- @todo: add coverage badge details -->

<h2 id="e2e-testing" class="anchor-heading">E2E Testing {% include Util/link_anchor anchor="e2e-testing" %} {% include Util/top %}</h2>

### Testing environment

The environment should be accessible and easy to set up in both local and CI environments. In the WordPress context, the environment must also be configurable to fit as many scenarios as possible, including testing against different WP versions and with other plugins/themes activated. For the open-source projects, we also want to use a community-driven tool. Because of those reasons, we choose `wp-env` for 10up's Open Source projects.

### Test runner

Cypress is the tool we're using for E2E testing. Cypress provides a great developer experience for writing the tests, including simple and familiar syntax and a powerful visual debugger. On top of that, Cypress gives us the most consistent results among the tools we tried.

### Importing the test URL

In most cases, the URL of the test instance is `http://localhost:8889`. But this can be changed, so instead of hard-coding the URL, we import it from `wp-env` and merge it into Cypress config.

```js
// tests/cypress/plugins/index.js
const { readConfig } = require( '@wordpress/env/lib/config' );
/**
 * @type {Cypress.PluginConfig}
 */
module.exports = async ( on, config ) => {
	wpEnvConfig = await readConfig( 'wp-env' );
	if ( wpEnvConfig ) {
		const port = wpEnvConfig.env.tests.port || null;
		if ( port ) {
			config.baseUrl = wpEnvConfig.env.tests.config.WP_TESTS_DOMAIN;
		}
	}
	return config;
};
```

Then in testcases, we can safely omit the URL:
```js
cy.visit( `/wp-admin` );
```

### Testing against multiple configurations

The purpose of E2E testing is to ensure the user-facing features work as expected. In the WordPress context, we can extend that purpose to "working as expected against supported WP versions and plugins/themes". At 10up, we're using GitHub Actions matrix and `wp-env` config override to solve that problem by [generating `wp-env` config](https://github.com/10up/simple-podcasting/blob/develop/tests/bin/set-core-version.js) for [each matrix](https://github.com/10up/simple-podcasting/blob/develop/.github/workflows/test-branch.yml#L30-L31). We're doing it for WP core version only, but it can be adapted and updated to handle more complex configurations.
