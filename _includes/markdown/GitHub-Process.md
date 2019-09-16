The following items are required across all repositories managed by our Open Source Practice team.  By keeping the same experience across all our repositories, it makes it easier for 10uppers and external contributors to work within any repository and operate with the same assumptions as any other 10up repository.

<h2 id="issue-pr-labels" class="anchor-heading">Issue and PR labels {% include Util/link_anchor anchor="issue-pr-labels" %} {% include Util/top %}</h2>

The following labels will our standard set of labels across all open source repositories to help ensure we use clear and consistent labelling terminology.  This will allow us to see the status and type of all issues at a glance, to help track and report on contributions across our repositories, and to provide easier ways to find issues to contribute to (e.g., all `needs:ux` and `good-first-issues`).  We’re starting a minimal set of labels and will let progressive enhancement further define them for us as well as perform occasional housekeeping.
- `type:bug` - “Something isn't working.” (color: #d73a4a)
- `type:enhancement` - “New feature or request.” (color: #a2eeef)
- [`type:good-first-issue`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Atype%3Agood-first-issue) - “Good for newcomers.” (color: #993299)
- `type:question` - “Further information is requested.” (color: #d876e3)
- [`needs:engineering`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Aengineering+) - “This requires engineering to resolve.” (color: #999999)
- [`needs:code-review`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Acode-review+) - “This requires code review.” (color: #999999)
- [`needs:design`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Adesign+) - “This requires design to resolve.” (color: #999999)
- [`needs:documentation`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Adocumentation+) - “This requires documentation.” (color: #999999)
- [`needs:feedback`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Afeedback+) - “This requires feedback to determine next steps.” (color: #999999)
- [`needs:refresh`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Arefresh+) - “This requires a refreshed PR to resolve.” (color: #999999)
- [`needs:tests`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Atests+) - “This requires tests.” (color: #999999)
- [`needs:ux`](https://github.com/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+user%3A10up+no%3Aassignee+label%3Aneeds%3Aux+) - “This requires user experience to resolve.” (color: #999999)
- `resolution:not-applicable` - “We do not feel this issue is valid.” (color: #FFA500)
- `resolution:not-reproducible` - “We are unable to reproduce this issue.” (color: #FFFF00)
- `resolution:resolved` - “This issue has been resolved.” (color: #008000)
- `resolution:wontfix` - “We do not intend to resolve this issue.” (color: #000000)

<h2 id="milestones" class="anchor-heading">Milestones {% include Util/link_anchor anchor="milestones" %} {% include Util/top %}</h2>

We are also adding the following set of milestones across our open source repositories to help give some clarity to the priority of our work (e.g., numbered milestone has priority, Future Release has low priority).  When it comes to using numbered milestones (e.g., 1.3.7), we follow the Semantic Versioning as noted in the [10up Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#workflows).
- Future Release - Not planned for an upcoming major, minor, or patch release.
All repositories should also have at least one numbered milestone available that shows work planned for an upcoming release:
- Next Major Release - Our next release potentially with breaking changes.
- Next Minor Release - Our next backwards-compatible new functionality release.
- Next Patch Release - Our next backwards-compatible bugfix release.

<h2 id="branching-merging-deploying" class="anchor-heading">Branching, Merging, and Deploying {% include Util/link_anchor anchor="branching-merging-deploying" %} {% include Util/top %}</h2>

Each repository should have a `master` and `develop` branch with `develop` being the default branch.  [Branching and Deploying should follow the processes outlined in the Engineering Best Practices for plugins](https://10up.github.io/Engineering-Best-Practices/version-control/#plugins).  Similarly, we should [protect the `master` branch as outlined in the Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#protecting-the-master-branch).  Merges should be handled as [non-fast-forwards merges as outlined in the Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/version-control/#merges) and not squash merges so that the `master` branch maintains full commit and code author history, this is done for transparency and to honor all contributions to our open source work.
This means that we’ll want the following GitHub settings:
- Settings > Options > Merge button: Allow merge commits
- Settings > Options > Merge button: [DISABLE] Allow squash merging
- Settings > Options > Merge button: Allow rebase merging
- Settings > Branches > Default branch: `develop`
- Settings > Branches > Branch protection rules > `master` ...AND… `develop`:
  - Require pull request reviews before merging, Required approving reviews: 1
  - Dismiss stale pull request approvals when new commits are pushed
  - [DISABLE] Require review from Code Owners
  - [DISABLE] Restrict who can dismiss pull request reviews
  - Require status checks to pass before merging
  - [DISABLE] Require branches to be up to date before merging
  - [DISABLE] Filters for GitHub Actions
  - continuous-integration/travis-ci
  - [DISABLE] tag
  - [DISABLE] Require signed commits
  - [DISABLE] Include administrators
  - [DISABLE] Restrict who can push to matching branches

<!-- @todo: add screenshot of these settings from GitHub -->

<h2 id="documentation" class="anchor-heading">Documentation {% include Util/link_anchor anchor="documentation" %} {% include Util/top %}</h2>

Maintain documentation in the same repository as much as possible. This keeps everything portable and usable even when offline. There are two main varieties of documentation typically associated with open source software: usage instructions and maintenance guidelines. Most of this section focuses on maintenance guidelines to support the process you’ve outlined, as usage instructions will vary widely between projects.

Depending on the amount of documentation associated with your projects usage instructions, you may find that hosting them as a separate view, such as [GitHub Pages](https://pages.github.com/) or a [GitHub wiki](https://help.github.com/en/articles/about-wikis), is preferable to markdown files in a `/docs/` subfolder.  Note that if you go the GitHub Pages route, that you'll want to consider a `gh-pages` branch that deploys to your GitHub Pages site.

<!-- @todo: WIKI tips: wiki repo (don’t submodule...), wiki repo strategies and examples -->
