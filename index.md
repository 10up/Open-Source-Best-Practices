---
page: introduction
title: Introduction
nav: Home
group: navigation
weight: 1
layout: default
subnav:
  - title: Why OSS?
    tag: why-oss
  - title: OSS for Agencies
    tag: agencies
  - title: Open Source vs. Open Process
    tag: process
  - title: Contributing
    tag: contributing
updated: 16 Sep 2019
---

<div class="toc">
	<header>
		<h2>Table of Contents</h2>
	</header>

	<div class="col">
		<h3><a href="{{ site.baseurl }}#top">Introduction</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}#why-oss">Why OSS?</a></li>
			<li><a href="{{ site.baseurl }}#agencies">OSS for Agencies</a></li>
			<li><a href="{{ site.baseurl }}#process">Open Source vs. Open Process</a></li>
			<li><a href="{{ site.baseurl }}#contributing">Contributing</a></li>
		</ul>
	</div>

    <div class="col">
		<h3><a href="{{ site.baseurl }}/releasing/#top">Releasing Code</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/releasing/#licensing">Licensing</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#client-permissions">Client Permissions</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#choosing-tools">Choosing Tools</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#accessibility">Accessibility</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#security">Security</a></li>
			<li><a href="{{ site.baseurl }}/releasing/#release-process">Release Process</a></li>
		</ul>
	</div>

	    <div class="col">
  		<h3><a href="{{ site.baseurl }}/maintaining/#top">Maintenance Process</a></h3>
  	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/community/#top">Community</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/community/#readme">Readme</a></li>
			<li><a href="{{ site.baseurl }}/community/#code-of-conduct">Code of Conduct</a></li>
			<li><a href="{{ site.baseurl }}/community/#contributing-guidelines">Contributing Guidelines</a></li>
		</ul>
	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/version-control/#top">Version Control</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/version-control/#structure">Structure</a></li>
			<li><a href="{{ site.baseurl }}/version-control/#workflows">Workflows</a></li>
		</ul>
	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/github-process/#top">GitHub Process</a></h3>
	</div>
</div>

<div class="docs-section">
		{% capture introduction %}{% include markdown/Introduction.md %}{% endcapture %}
		{{ introduction | markdownify }}
</div>
