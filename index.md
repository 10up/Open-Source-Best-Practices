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
		<h3><a href="{{ site.baseurl }}/starting/#top">Starting or Releasing a Project</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/starting/community/#readme">README.md Best Practices</a></li>
			<li><a href="{{ site.baseurl }}/starting/releasing/#licensing">License File</a></li>
			<li><a href="{{ site.baseurl }}/starting/community/#contributing">Contribution Guidelines</a></li>
			<li><a href="{{ site.baseurl }}/starting/community/#code-of-conduct">Code of Conduct</a></li>
			<li><a href="{{ site.baseurl }}/starting/releasing/#changelog">Semantic Versioning & Release Tags</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/github-process/#issue-pr-labels">Initial Repo Setup</a></li>
		</ul>
	</div>

	<div class="col">
  		<h3><a href="{{ site.baseurl }}/maintaining/#top">Maintaining, Supporting, and Enhancing</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/starting/releasing/#changelog">CHANGELOG Standards</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/github-process/#issue-pr-labels">Issue Triage & Labeling</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/maintaining/#issue-pr-mgmt">Pull Request Guidelines</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/github-process/#continuous-integration">Continuous Integration / Testing</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/github-process/#documentation">Documentation Standards</a></li>
			<li><a href="{{ site.baseurl }}/starting/releasing/#security">Security Handling</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/maintaining/#maintainers-contributors">Communication Best Practices</a></li>
		</ul>
  	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/growing/#top">Growing and Sustaining a Project</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/growing/#governance">Governance Models</a></li>
			<li><a href="{{ site.baseurl }}/starting/releasing/#credit-management">Community Recognition</a></li>
			<li><a href="{{ site.baseurl }}/maintaining/github-process/#milestones">Roadmaps & Planning</a></li>
			<li><a href="{{ site.baseurl }}/growing/#sponsorships">Sponsorships / Funding</a></li>
			<li><a href="{{ site.baseurl }}/growing/#succession">Succession Planning</a></li>
			<li><a href="{{ site.baseurl }}/growing/#sunsetting">Sunsetting/Archiving Projects</a></li>
		</ul>
	</div>

	<div class="col">
		<h3><a href="{{ site.baseurl }}/references/#top">References and Resources</a></h3>
		<ul>
			<li><a href="{{ site.baseurl }}/references/#tools">Recommended Tools & Services</a></li>
			<li><a href="{{ site.baseurl }}/references/#standards">External Standards (SPDX, OSI, SemVer)</a></li>
			<li><a href="{{ site.baseurl }}/references/#examples">Example Repositories</a></li>
		</ul>
	</div>
</div>

<div class="docs-section">
		{% capture introduction %}{% include markdown/Introduction.md %}{% endcapture %}
		{{ introduction | markdownify }}
</div>
