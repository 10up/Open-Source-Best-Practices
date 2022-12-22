<h2 id="maintainers-contributors" class="anchor-heading">Maintainers and Contributors {% include Util/link_anchor anchor="maintainers-contributors" %} {% include Util/top %}</h2>

When maintaining an open source project, there is a need to have at least one person listed as the "Maintainer".  The rationale for having a Maintainer role for an open source project is because it:

- Allows an individual to become an expert in one or more project. They can then be a "go to" when other engineers have questions internally, when clients have questions, when questions come in on GitHub or WordPress.org, etc.
- When multiple people act as a Maintainer on a project and responsibility is not shared by a small group across all open source projects it allows us to (hopefully!) release more frequently across our projects
- Gives engineers a more concrete trajectory to work towards as far as career progress goes
- Gives engineers the chance to develop skills like communication, providing proper feedback, better testing/reviewing skills, responsibility to get a quality release out, etc. Things they would naturally be learning on client and other projects that they might otherwise not have as many opportunities to work on

The Maintainer role can also be seen as an alternative to a typical "Technical Lead" role on client delivery projects in that it expects someone to help mentor and guide others towards a shared outcome for a project while also helping shape a project's roadmap and provide technical review of implementation details.  Maintainers are listed in a project's CREDITS.md file in the Maintainers section (e.g., [Distributor](https://github.com/10up/distributor/blob/develop/CREDITS.md)) as well as in a WordPress plugin's readme.txt file in the Contributors section (e.g., [Winamp Block](https://github.com/10up/retro-winamp-block/blob/develop/readme.txt)).  Inactive Contributors listed in the readme.txt file will only be removed at their request as we otherwise keep them listed as continued thanks for their historical maintainer efforts.

Similarly, central to a successful open process are setting expectations and respecting the time of other participants, especially when they are volunteers or "Contributors".  The following are expectations in how to communicate with and recognize the efforts from contributors on open source projects.

- Include a [CONTRIBUTING.md file](https://10up.github.io/Open-Source-Best-Practices/community/#contributing) outlining ways to contribute to a project helps non-maintainers understand how best to contribute.
- Be thankful and specific when including participants, from acknowledging a well-defined issue or a pull request they've opened, to including them in [changelog release notes](https://10up.github.io/Open-Source-Best-Practices/releasing/#changelog) and the [CREDITS.md file](https://10up.github.io/Open-Source-Best-Practices/releasing/#credit-management).
- Recognize that opening an issue or pull request doesn't necessarily indicate additional time to continue triaging an issue or updating a pull request based on code review / feedback, so you may need to pick up and cover those as a maintainer.

<h2 id="issue-pr-mgmt" class="anchor-heading">Issue and Pull Request Management {% include Util/link_anchor anchor="issue-pr-mgmt" %} {% include Util/top %}</h2>

In the [2017 Open Source Survey conducted by GitHub](https://opensourcesurvey.org/2017/), the number one issue that people feel is most important for open source projects is “responsive maintainers.”  As such, we should aim for quick response and triage on all newly opened issues and pull requests.  Not so much that we quickly resolve those issues or merge those pull requests, but that we respond quickly and set realistic expectations for what contributors can expect from us.

We have set up default [Issue](https://github.com/10up/.github/tree/trunk/ISSUE_TEMPLATE) and [Pull Request](https://github.com/10up/.github/blob/trunk/PULL_REQUEST_TEMPLATE.md) Templates in the [10up .github repository](https://github.com/10up/.github), so feel free to let those do the work, or create custom ones for your repository (example: [ClassifAI](https://github.com/10up/classifai/tree/develop/.github)).

Issue triage will primarily be handled by our Open Source Practice leadership as well as specifically identified Maintainers for each project, but to help ensure we reply to all issues and pull requests within five business days, others within 10up are always welcome to assist with triage.  We ask that as you review issues and pull requests you consider the following:

- When someone new lands on a project, thank them for their interest! GitHub shows various first-time contributor indicators.
- Utilize our [10up Saved Replies](https://github.com/10up/.github/blob/trunk/.github/SAVED_REPLIES.md) to quickly respond to standard requests.
- Apply labels to ensure others who review issues and pull requests after you can benefit from your initial triage.
- If a pull request hasn't been linked to an existing issue, please add a comment to link them or open a corresponding issue.
- As issues come in via WordPress.org support requests, respond with a “thanks for your report…”, let them know you're moving the forum report to GitHub, and then provide them the link to the newly opened GitHub issue.

The following GitHub Actions are also recommended on most, if not all, projects:

- [Deploying a plugin to the WordPress.org repository](https://github.com/10up/action-wordpress-plugin-deploy) ([example](https://github.com/10up/eight-day-week/blob/develop/.github/workflows/push-deploy.yml))
- [Deploying plugin asset/readme updates to the WordPress.org repository](https://github.com/10up/action-wordpress-plugin-asset-update) ([example](https://github.com/10up/eight-day-week/blob/develop/.github/workflows/push-asset-readme-update.yml))
- [PHP linting without additional codebase dependencies](https://github.com/10up/wpcs-action) ([example](https://github.com/10up/classifai/blob/develop/.github/workflows/lint.yml))
- [Publishing generated hook documentation to GitHub Pages](https://github.com/10up/actions-wordpress/blob/stable/hookdocs-workflow.md) ([example](https://github.com/10up/distributor/blob/develop/.github/workflows/build-docs.yml))
- [No Response issue auto-closer](https://github.com/lee-dohm/no-response) ([example](https://github.com/10up/ads-txt/blob/develop/.github/workflows/no-response.yml))

<h2 id="dotorg-support-reps" class="anchor-heading">WordPress.org Support {% include Util/link_anchor anchor="dotorg-support" %} {% include Util/top %}</h2>

We recommend limiting the number of accounts that have access to your plugin on WordPress.org SVN, as this reduces potential attack vectors and minimizes the risk of bad actors nefariously affecting your code.  The downside to this is that the nice “Plugin Author” label and highlight that appears alongside messages from plugin contributors as well as the ability to mark threads as resolved or sticky within the forums is limited to that small number of accounts.  Not to worry, you can use [Plugin Support Reps](https://make.wordpress.org/plugins/2017/09/04/plugin-support-reps/) to add others on your team who will then appear with a nice “Plugin Support” label and highlight alongside their messages in the forums.  Support reps can also mark threads as resolved or sticky, but will not have commit access to the plugin codebase on SVN.  You can assign support reps on the Advanced View on your plugin pages (e.g., https://wordpress.org/plugins/restricted-site-access/advanced/).

When a support topic has been resolved, ensure that you change the `Status` from `not resolved` to `resolved`.  If a support response has been left on an open topic, but there is no response or update from the original reporter then the best approach is to leave a final comment after 30 days noting any additional information or feedback and that the topic is being closed "due to inactivity" and note that subsequent updates can be tracked in a new issue as additional information becomes available.

<h2 id="slack-channel-github-activity" class="anchor-heading">Slack channel to track GitHub activity {% include Util/link_anchor anchor="slack-channel-github-activity" %}</h2>

In the scenario where your organization uses GitHub for code and Slack for communications, then integrating the two seems reasonable.  In this case, we recommend setting up a dedicated channel to track activity within your GitHub Organization using the `/github subscribe owner/repository` [Slack command](https://get.slack.help/hc/en-us/articles/232289568-GitHub-for-Slack).  Even further, utilize the `/github subscribe owner/repository issues, pulls, releases, deployments, reviews, comments, discussions` command to ensure you’re alerted to comments or discussions that come into your project repositories.  Once GitHub feeds are set up, we also recommend utilizing a specific [Slack emoji reaction](https://get.slack.help/hc/en-us/articles/206870317-Emoji-reactions) to note that someone from your team will take responsibility for that specific activity ([example](https://slackmojis.com/emojis/1588-onit/)).

<h2 id="slack-channel-dotorg-activity" class="anchor-heading">Slack channel to track WordPress.org plugin support/forum activity {% include Util/link_anchor anchor="slack-channel-dotorg-activity" %}</h2>

In the scenario where your organization uses GitHub for code and publishes code to the WordPress.org repository, then integrating the two seems reasonable.  In this case, then we recommend setting up a dedicated channel to track activity across your suite of plugins and themes using the [RSS Feeds functionality](https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack).  More specifically, you’ll want to pull up your Support page ([plugin example](https://wordpress.org/support/plugin/elasticpress/), [theme example](https://wordpress.org/support/theme/twentynineteen/)) and Review page ([plugin example](https://wordpress.org/plugins/elasticpress/#reviews), [theme example](https://wordpress.org/support/theme/twentynineteen/reviews/)) and then add /feed/ to the end of the URL that you utilize for the RSS Feed subscription ([Support example](https://wordpress.org/support/plugin/elaticpress/feed/), [Review example](https://wordpress.org/support/plugin/elasticpress/reviews/feed/)).  Once RSS feeds are set up, we also recommend utilizing a specific [Slack emoji reaction](https://get.slack.help/hc/en-us/articles/206870317-Emoji-reactions) to note that someone from your team will take responsibility for that specific post ([example](https://slackmojis.com/emojis/1588-onit/)).

<h2 id="version-control" class="anchor-heading">Version Control {% include Util/link_anchor anchor="version-control" %}</h2>

In general we follow the [Version Control guidelines from the 10up Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#top) including the approaches for [structure](https://10up.github.io/Engineering-Best-Practices/version-control/#structure-package-management) and [workflows](https://10up.github.io/Engineering-Best-Practices/version-control/#workflows).

<h2 id="version-control" class="anchor-heading">WordPress and PHP Minimums {% include Util/link_anchor anchor="wp-php-mins" %}</h2>

Our defined minimum supported versions for WordPress and PHP are set as follows:

- The active major version of WordPress from one year prior (e.g. when [6.0](https://wordpress.org/news/2022/05/arturo/) was released this would mean [5.7](https://wordpress.org/news/2021/03/esperanza/) is minimum supported version)
- PHP version 7.4

The WordPress minimum can be updated with each subsequent [major version release](https://wordpress.org/about/history/), noting that depending on the release velocity of the prior year that the minimum may not change or may increase by more than one version.

We expect to review the PHP minimum heading into 2023 and bump that to 8.0 (with the coming end-of-life support of 7.4 and increase in [WordPress core support for 8.0+](https://make.wordpress.org/core/handbook/references/php-compatibility-and-wordpress-versions/)).  PHP supported versions and end-of-life timelines can be viewed on the [PHP Supported Versions page](https://www.php.net/supported-versions).
