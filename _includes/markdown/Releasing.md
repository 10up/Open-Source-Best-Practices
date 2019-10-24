<h2 id="naming" class="anchor-heading">Naming {% include Util/link_anchor anchor="naming" %} {% include Util/top %}</h2>

Avoid name conflicts if at all possible.  [Check for open source projects with a similar name](http://ivantomic.com/projects/ospnc/).  Make sure that the name doesn’t [infringe upon any trademarks](http://www.wipo.int/branddb/en/).  Do a Google search for your project name to ensure that something else doesn’t appear in the search results that might negatively reflect on your project.

Aim for conceptual clarity over cleverness and puns. Creativity is good, but a name that also clearly explains or at least suggests what the software being released **actually does** is better.

<h2 id="licensing" class="anchor-heading">Licensing {% include Util/link_anchor anchor="licensing" %} {% include Util/top %}</h2>

At 10up, any project that is a WordPress plugin or theme should be licensed [GPLv2](https://opensource.org/licenses/GPL-2.0).  Standalone JavaScript libraries or modules can be licensed [MIT](https://opensource.org/licenses/MIT).  We recommend this route as a default, but any other included libraries and integrations must also be taken into consideration before making a final licensing decision.

<h2 id="client-permissions" class="anchor-heading">Client permissions {% include Util/link_anchor anchor="client-permissions" %} {% include Util/top %}</h2>

Open-sourcing code that has been developed as part of a client project can be complex. Many agency contracts (including many at 10up) define the work product as "work for hire" and grant copyright over the code produced to the client. In those cases, specific permission from the client is required in order to release any code developed on the projects governed by that contract.

That said, clients benefit as much as anyone (perhaps even more than anyone) when functionality developed as a part of their project can be released into open source or contributed back to the projects which it extends or builds upon. They get the benefit of ongoing community contribution, testing, and maintenance, and don't have to shoulder the maintenance of that new plugin or feature themselves.

If you have identified code developed as part of a client project that would make an ideal contribution to an existing open source project or an open source release of its own, work with your account manager to specifically identify the need for and obtain client permission.

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

<h2 id="release-process" class="anchor-heading">Release Process {% include Util/link_anchor anchor="release-process" %} {% include Util/top %}</h2>

All releases should follow one of two release processes we’ve crafted (see [Ads.txt](https://github.com/10up/ads-txt/blob/develop/CONTRIBUTING.md#release-instructions) and [Distributor](https://github.com/10up/distributor/blob/develop/CONTRIBUTING.md#release-instructions)) or even more simply, leverage a GitHub Action to automate the release and deploy to WordPress.org as necessary (see [Restricted Site Access](https://github.com/10up/restricted-site-access/blob/develop/.github/main.workflow)).  If this is a major release, we should consider publishing an update post on 10up.com/blog and updating any related microsites.

Once a release has been tagged on GitHub, include the link to the release tag in the related milestone, ensure the milestone date is accurate, move any remaining open issues or PRs from the milestone to a future milestone, remove any closed but unmerged PRs from the milestone, and then close the milestone.

<h2 id="changelog" class="anchor-heading">Changelog {% include Util/link_anchor anchor="changelog" %} {% include Util/top %}</h2>

We will maintain a changelog in its own CHANGELOG.md file, linked from the [README.md file](https://10up.github.io/Open-Source-Best-Practices/community/#readme), follows the [Keep a Changelog standard](https://keepachangelog.com/en/1.0.0/), and adheres to [Semantic Versioning](http://semver.org/) as described in the [10up Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#workflows).  See [Restricted Site Access](https://github.com/10up/restricted-site-access/blob/develop/CHANGELOG.md) and [Simple Local Avatars](https://github.com/10up/simple-local-avatars/blob/develop/CHANGELOG.md) as an example.  When building a changelog for a release, append any props to properly credit individuals who contributed to each item (see [ClassifAI example](https://github.com/10up/classifai/blob/develop/CHANGELOG.md#140---2019-09-26)).

<h2 id="credit-management" class="anchor-heading">Team and Credit Management {% include Util/link_anchor anchor="credit-management" %} {% include Util/top %}</h2>

We should add a CREDITS.md file that lists maintainers, contributors (in chronological order of contribution), and optionally any libraries utilized by the plugin/tool (example: [Insert Special Characters](https://github.com/10up/insert-special-characters/blob/develop/CREDITS.md)).  While the concept of the [All Contributors spec](https://github.com/all-contributors/all-contributors) is nice, the implementation and layout can get a bit complex and none of our plugins/tools have a large enough contribution audience to warrant the broad [contribution types / emoji key](https://allcontributors.org/docs/en/emoji-key) used in the spec.  As such, the CREDITS.md file should be linked from the README.md file and should be laid out like this:

`The following acknowledges the Maintainers for this repository, those who have Contributed to this repository (via bug reports, code, design, ideas, project management, translation, testing, etc.), and any Libraries utilized.`

`## Maintainers`

`The following individuals are responsible for curating the list of issues, responding to pull requests, and ensuring regular releases happen.`

`[Display Name](GitHub profile link), [Display Name2](GitHub profile link2), … , [Display NameN](GitHub profile linkN).`

`## Contributors`

`Thank you to all the people who have already contributed to this repository via .`

`[Display Name](GitHub profile link), [Display Name2](GitHub profile link2), … , [Display NameN](GitHub profile linkN).`

`## Libraries`

`The following software libraries are utilized in this repository.`

`[Library Name](library link), [Library Name2](library link2), … , [Library NameN](library linkN).`
