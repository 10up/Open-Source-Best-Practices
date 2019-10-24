Central to a successful open process are setting expectations and respecting the time of other participants, especially when they are volunteers.

<!-- @todo: add additional, missing? bullets here-->
- Be thankful and specific when including participants, whether that is…?

<h2 id="issue-pr-mgmt" class="anchor-heading">Issue and Pull Request Management {% include Util/link_anchor anchor="issue-pr-mgmt" %} {% include Util/top %}</h2>

In the [2017 Open Source Survey conducted by GitHub](https://opensourcesurvey.org/2017/), the number one issue that people feel is most important for open source projects is “responsive maintainers.”  As such, we should aim for quick response and triage on all newly opened issues and pull requests.  Not so much that we quickly resolve those issues or merge those pull requests, but that we respond quickly and set realistic expectations for what contributors can expect from us.

We have setup default [Issue](https://github.com/10up/.github/tree/master/ISSUE_TEMPLATE) and [Pull Request](https://github.com/10up/.github/blob/master/PULL_REQUEST_TEMPLATE.md) Templates in the [10up .github repository](https://github.com/10up/.github), so feel free to just utilize those or create custom ones for your repository (example: [ClassifAI](https://github.com/10up/classifai/tree/develop/.github)).

Issue triage will primarily be handled by our Open Source Leadership, but in order to ensure we reply to all issues and pull requests within five business days others within 10up are welcome to assist with triage.  We ask that as you review issues and pull requests that you consider the following:

<!-- @todo: add additional considerations here-->
- When someone new lands on your project, thank them for their interest!
- ...for .org support requests, (“thanks for report…”), moving forum report to GH...
- ...

<h2 id="dotorg-support-reps" class="anchor-heading">WordPress.org Support Reps {% include Util/link_anchor anchor="dotorg-support-reps" %} {% include Util/top %}</h2>

We recommended limiting the number of accounts that have access to your plugin on WordPress.org SVN, as this reduces potential attack vectors and minimizes the risk of bad actors nefariously affecting your code.  The downside to this is that the nice “Plugin Author” label and highlight that appears alongside messages from plugin contributors as well as the ability to mark threads as resolved or sticky within the forums is limited to that small number of accounts.  Not to worry, you can utilize [Plugin Support Reps](https://make.wordpress.org/plugins/2017/09/04/plugin-support-reps/) to add others on your team to appear with a nice “Plugin Support” label and highlight alongside their messages in the forums.  Support reps can also mark threads as resolved or sticky, but won’t have commit access to the plugin codebase on SVN.  Set those support reps on the Advanced View on your plugin pages!

<h2 id="slack-channel-github-activity" class="anchor-heading">Slack channel to track GitHub activity {% include Util/link_anchor anchor="slack-channel-github-activity" %}</h2>

In the scenario where your organization utilizes GitHub for code and Slack for communications, then integrating the two seems reasonable.  In this case, we recommend setting up a dedicated channel to track activity within your GitHub Organization using the `/github subscribe owner/repository` [Slack command](https://get.slack.help/hc/en-us/articles/232289568-GitHub-for-Slack).  Even further, utilize the `/github subscribe owner/repository reviews comments branches commits:all` command to ensure you’re alerted to comments or commits that come into your project repositories.  Once GitHub feeds are setup, we also recommend utilizing a specific [Slack emoji reaction](https://get.slack.help/hc/en-us/articles/206870317-Emoji-reactions) to note that someone from your team will take responsibility for that specific activity ([example](https://emojipedia.org/pushpin/)).

<h2 id="slack-channel-dotorg-activity" class="anchor-heading">Slack channel to track WordPress.org plugin support/forum activity {% include Util/link_anchor anchor="slack-channel-dotorg-activity" %}</h2>

In the scenario where your organization utilizes GitHub for code and publishes code to the WordPress.org repository, then integrating the two seems reasonable.  In this case, then we recommend setting up a dedicated channel to track activity across your suite of plugins and themes using the [RSS Feeds functionality](https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack).  More specifically, you’ll want to pull up your Support page ([plugin example](https://wordpress.org/support/plugin/elasticpress/), [theme example](https://wordpress.org/support/theme/twentynineteen/)) and Review page ([plugin example](https://wordpress.org/plugins/elasticpress/#reviews), [theme example](https://wordpress.org/support/theme/twentynineteen/reviews/)) and then add /feed/ to the end of the URL that you utilize for the RSS Feed subscription ([Support example](https://wordpress.org/support/plugin/elaticpress/feed/), [Review example](https://wordpress.org/support/plugin/elasticpress/reviews/feed/)).  Once RSS feeds are setup, we also recommend utilizing a specific [Slack emoji reaction](https://get.slack.help/hc/en-us/articles/206870317-Emoji-reactions) to note that someone from your team will take responsibility for that specific post ([example](https://emojipedia.org/pushpin/)).

<h2 id="version-control" class="anchor-heading">Version Control {% include Util/link_anchor anchor="version-control" %}</h2>

In general we follow the [Version Control guidelines from the 10up Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#top) including the approaches for [structure](https://10up.github.io/Engineering-Best-Practices/version-control/#structure-package-management) and [workflows](https://10up.github.io/Engineering-Best-Practices/version-control/#workflows).
