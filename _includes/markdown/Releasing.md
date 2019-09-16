<h2 id="readme" class="anchor-heading">Readme {% include Util/link_anchor anchor="readme" %} {% include Util/top %}</h2>

A README, Code of conduct, Contributing, License, Security policy, Issue templates, and Pull request template should all exist on each repository.  The 10up standard for each of these (except README and LICENSE) are noted in the [10up .github repository](https://github.com/10up/.github) and will appear in all 10up repositories unless a local one is created so feel free to leverage the default files unless it's necessary and reasonable to create custom ones local to your repository.

### README outline

Each README.md file should follow a similar outline including the items below (as feasible and makes sense).

#### Title and Description

Ideally we have a (less than 100px in height) logo image we can use with the repository name as fallback.  Below that should be the description in pullquote form.  Finally any applicable badges for the repository should be displayed (e.g., build status, code coverage, stable release version, support level, WP tested up to, license, dependencies, number of contributors).

#### Features

List short bulleted items on the major features/benefits of the plugin/toolkit.  After the bulleted list, we should end with “For more details on changes in each release, check out CHANGELOG.md.”

#### Requirements

This is an optional section, but should be included and list WordPress, PHP, etc. versions that are required as well as any additional plugins/themes/etc. for the plugin/tool to function properly.

#### Installation

This is an optional section, but should include any unique install steps besides the normal “search in WP Admin” / “upload ZIP” steps.

#### Setup

This is an optional section, but should include simple screenshots and basic instructions for any setup or settings required to configure the plugin/tool.

#### Support Level

<!-- @todo: needs proper link on "Support Levels" -->
Check the “Support Levels” section for details on what to include here.

#### Known Caveats / Issues

This is an optional section, but should include any issues, bugs, or things to note about the plugin/tool that a user might encounter while using it.

#### Changelog

<!-- @todo: add details for this section-->

#### Contributing

Verbatim with correct MD file links: “Please read CODE_OF_CONDUCT.md for details on our code of conduct, CONTRIBUTING.md for details on the process for submitting pull requests to us, and CREDITS.md for a list of maintainers, contributors, and libraries used in this repository.”

#### 10up promo

At the end of the README should be the standard 10up Hiring promotion image with a link back to https://10up.com/contact/.  See examples on [Distributor](https://github.com/10up/distributor/#like-what-you-see) and [ClassifAI](https://github.com/10up/classifai#like-what-you-see).

<h2 id="code-of-conduct" class="anchor-heading">Code of Conduct {% include Util/link_anchor anchor="code-of-conduct" %} {% include Util/top %}</h2>

@todo

<h2 id="contributing" class="anchor-heading">Contributing {% include Util/link_anchor anchor="contributing" %} {% include Util/top %}</h2>

@todo


<h2 id="licensing" class="anchor-heading">Licensing {% include Util/link_anchor anchor="licensing" %} {% include Util/top %}</h2>

At 10up, the vast majority of our open sourced code is released under the [MIT license](https://opensource.org/licenses/MIT), which is highly permissive and compatible with integration into GPL software such as WordPress. We recommend this route as a default but any other included libraries and integrations must also be taken into consideration before making a final licensing decision.  

<h2 id="client-permissions" class="anchor-heading">Client permissions {% include Util/link_anchor anchor="client-permissions" %} {% include Util/top %}</h2>

Best scenario / shared goals, afterthoughts…

In order to be publicly open sourced, all new plugins should have Gutenberg support and must conform with the [WCAG 2.0 guidelines at level AA](https://www.w3.org/TR/WCAG20/).

<h2 id="choosing-tools" class="anchor-heading">Choosing tools {% include Util/link_anchor anchor="choosing-tools" %} {% include Util/top %}</h2>

Repository hosting and issue management are separate considerations, but for convenience and familiarity we host and manage open source code on GitHub and are active participants in [their maintainer community](https://github.com/maintainers/welcome). WordPress plugins are generally also mirrored onto the SVN-backed [WordPress.org Plugin Repository](https://wordpress.org/plugins), where support requests are monitored and turned into GitHub issues where applicable.

GitHub’s strength and weakness is that it is very code and solution-focused. There are times where more specialized tools are necessary for including disciplines such as design; these are chosen based on needs and participants. Many of the following sections contain GitHub-specific guidance but are still broadly applicable to other tools for project and code management.

<h2 id="accessibility" class="anchor-heading">Accessibility {% include Util/link_anchor anchor="accessibility" %} {% include Util/top %}</h2>

All newly released code should adhere to the [WCAG 2.0](https://www.w3.org/TR/WCAG20/) AA level with the goal of working through existing code as time allows to bring it up to WCAG 2.0 AA levels.  Utilize [checklists](https://www.wuhcag.com/wcag-checklist/) and [linters](https://pa11y.org/) to help ensure code released and updated adheres to these standards.

<h2 id="security" class="anchor-heading">Security {% include Util/link_anchor anchor="security" %} {% include Util/top %}</h2>

GitHub added support for [security alerts in November 2017](https://github.blog/2017-11-16-introducing-security-alerts-on-github/) and [automated security fixes in May 2019](https://github.blog/2019-05-23-introducing-new-ways-to-keep-your-code-secure/#automated-security-fixes-with-dependabot).  Both of these add up to additional help ensuring that your code is secure, so properly [list the packages that your repository depends on](https://help.github.com/en/articles/listing-the-packages-that-a-repository-depends-on) and [enable automated security fixes in your repository](https://help.github.com/en/articles/configuring-automated-security-fixes#managing-automated-security-fixes-for-your-repository).  If you have a private repository, then you’ll also need [to allow GitHub read-only access, to enable the dependency graph, and to enable security alerts](https://help.github.com/en/articles/opting-into-or-out-of-data-use-for-your-private-repository#opting-into-data-use-for-your-private-repository).  Finally, make sure to pay attention to your security alerts and work to build a release with those updates as reasonably expeditiously as possible.

Alongside security alerts and fixes, you should have a defined [security policy](https://help.github.com/en/articles/adding-a-security-policy-to-your-repository) in your repository.  This SECURITY.md file should provide clear instructions to contributors on how to responsibly report a security vulnerability and should describe how you report security vulnerabilities that are found.  We have setup a [default Security Policy](https://github.com/10up/.github/blob/master/SECURITY.md) in the [10up .github repository](https://github.com/10up/.github), so feel free to just utilize those or create custom ones for your repository (example: **TBD**).

This means that we’ll want the following GitHub settings:
- Settings > Options > Data services > Security alerts
- Settings > Security alerts > Organization and repository administrators
- Security > Alerts > Automated security fixes
