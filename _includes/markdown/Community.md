<h2 id="readme" class="anchor-heading">Readme {% include Util/link_anchor anchor="readme" %} {% include Util/top %}</h2>

A README, Code of conduct, Contributing guidelines, License, Security policy, Issue templates, and Pull request template should all exist in each repository.  The 10up standard for each of these (except README and LICENSE) is represented in the [10up .github repository](https://github.com/10up/.github) and will appear in all 10up repositories unless a local one is created, so feel free to leverage the default files unless it's necessary and reasonable to create custom ones for a given repository.

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

Check the [Support Levels](https://10up.github.io/Open-Source-Best-Practices/github-process/#support-levels) section for details on what to include here.

#### Known Caveats / Issues

This is an optional section, but should include any issues, bugs, or things to note about the plugin/tool that a user might encounter while using it.

#### Changelog

This is a required section, should link out to the respective CHANGELOG.md file, and should follow our documented approach within the CHANGELOG.md file as noted in the [Releasing Code section](https://10up.github.io/Open-Source-Best-Practices/releasing/#changelog).  See [ClassifAI](https://github.com/10up/classifai#changelog) as an example.

#### Contributing

Verbatim with correct MD file links: “Please read CODE_OF_CONDUCT.md for details on our code of conduct, CONTRIBUTING.md for details on the process for submitting pull requests to us, and CREDITS.md for a list of maintainers, contributors, and libraries used in this repository.”

#### 10up promo

At the end of the README should be the standard 10up Hiring promotion image with a link back to https://10up.com/contact/.  See examples on [Distributor](https://github.com/10up/distributor/#like-what-you-see) and [ClassifAI](https://github.com/10up/classifai#like-what-you-see).

<h2 id="code-of-conduct" class="anchor-heading">Code of Conduct {% include Util/link_anchor anchor="code-of-conduct" %} {% include Util/top %}</h2>

10up has standardized to the Contributor Covenant version of a Code of Conduct file, currently [version 1.4](https://www.contributor-covenant.org/version/1/4/code-of-conduct.html).  We also utilize the community-wide community health file functionality from GitHub, so any project that doesn't include it's own CODE_OF_CONDUCT.md file will inherit the [default 10up version](https://github.com/10up/.github/blob/master/CODE_OF_CONDUCT.md).  Projects may chose to include their own version of the Contributor Covenant CODE_OF_CONDUCT.md or rely upon the 10up default version.

<h2 id="contributing" class="anchor-heading">Contributing Guidelines {% include Util/link_anchor anchor="contributing" %} {% include Util/top %}</h2>

10up has standardized the ways in which we expect 10up, our project Maintainers, and community contributions to interrelate 
when contributing to our open source projects.  These are defined in our default [CONTRIBUTING.md file](https://github.com/10up/.github/blob/master/CONTRIBUTING.md) that will be inherited by any projects that do not have their own CONTRIBUTING.md file.  Projects may chose to include their own version of the CONTRIBUTING.md file or rely upon the 10up default version.
