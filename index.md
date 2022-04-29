---
page: introduction
title: Introduction
nav: Home
group: navigation
weight: 1
layout: default
subnav:
  - title: Introduction
    tag: intro
  - title: Why OSS?
    tag: why-oss
  - title: OSS for Agencies
    tag: agencies
  - title: Open Source vs. Open Process
    tag: process
  - title: Contributing to this guide
    tag: contributing
updated: 25 November 2019
---

<div class="toc">
	<header>
		<h2>Table of Contents</h2>
	</header>

	<div class="col">
		<h3><a href="{{ site.baseurl }}#top">Home</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}#intro">Introduction</a></li>		
			<li><a href="{{ site.baseurl }}#why-oss">Why OSS?</a></li>
			<li><a href="{{ site.baseurl }}#agencies">OSS for Agencies</a></li>
			<li><a href="{{ site.baseurl }}#process">Open Source vs. Open Process</a></li>
			<li><a href="{{ site.baseurl }}#contributing">Contributing to this guide</a></li>
		</ul>
	</div>

    	<div class="col">
		<h3><a href="{{ site.baseurl }}/releasing/#top">Releasing Code</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/releasing/#naming">Naming</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#licensing">Licensing</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#client-permissions">Client Permissions</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#choosing-tools">Choosing Tools</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#accessibility">Accessibility</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#security">Security</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#release-process">Release Process</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#changelog">Changelog</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#credit-management">Credit Management</a></li>
		</ul>
	</div>

	<div class="col">
  		<h3><a href="{{ site.baseurl }}/maintaining/#top">Maintenance Process</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/maintaining/#maintainers-contributors">Maintainers and Contributors</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/#issue-pr-mgmt">Issue and PR Management</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/#dotorg-support">WordPress.org Support</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/#slack-channel-github-activity">Tracking GitHub activity</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/#dslack-channel-dotorg-activity">Tracking WordPress.org activity</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/#version-control">Version Control</a></li>
		</ul>
  	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/community/#top">Community</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/community/#readme">Readme</a></li>
			<li><a href="{{ site.baseurl }}/community/#code-of-conduct">Code of Conduct</a></li>
			<li><a href="{{ site.baseurl }}/community/#contributing">Contributing Guidelines</a></li>
		</ul>
	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/github-process/#top">GitHub Process</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/github-process/#issue-pr-labels">Issue and PR labels</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#milestones">Milestones</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#branching-merging-deploying">Branching, Merging, and Deploying</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#documentation">Documentation</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#support-levels">Support Levels</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#opengraph-image">OpenGraph Image</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#dependency-management">Dependency Management</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#coding-standards">Coding Standards</a></li>
			<li><a href="{{ site.baseurl }}/github-process/#continuous-integration">Continuous Integration</a></li>
		</ul>
	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/testing/#top">Testing</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/testing/#code-coverage">Code Coverage</a></li>
			<li><a href="{{ site.baseurl }}/testing/#e2e-testing">E2E testing</a></li>
		</ul>
	</div>
</div>

<div class="docs-section">
		{% capture introduction %}{% include markdown/Introduction.md %}{% endcapture %}
		{{ introduction | markdownify }}
</div>
