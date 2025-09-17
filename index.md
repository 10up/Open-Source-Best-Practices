---
page: introduction
title: Open Source Best Practices
description: Guidance for every stage of your open source project.
nav: Home
group: navigation
weight: 1
layout: default
updated: 25 November 2019
---

<div class="docs-section">
	<header>
		<h1>Open Source Best Practices</h1>
		<p>Welcome! This guide helps you build and maintain healthy open source projects.<br>
		Choose the path that best fits where you are today:</p>
	</header>

	<div class="path-cards">
		<div class="path-card primary">
			<h2>🚀 Starting Your First Project</h2>
			<p>New to open source? Get your project off to a great start with these essentials:</p>
			<ul>
				<li><a href="{{ site.baseurl }}/starting/community/#readme">Set up your README and license</a></li>
				<li><a href="{{ site.baseurl }}/starting/community/#contributing">Add a Code of Conduct and contribution guidelines</a></li>
				<li><a href="{{ site.baseurl }}/starting/releasing/#release-process">Plan for your first release</a></li>
			</ul>
			<div class="path-cta">
				<a href="{{ site.baseurl }}/starting/" class="btn-primary">Explore the full <strong>Starting or Releasing a Project</strong> section »</a>
			</div>
		</div>

		<div class="path-card secondary">
			<h2>🔧 Maintaining an Existing Project</h2>
			<p>Already have a project? Keep it healthy and growing with these practices:</p>
			<ul>
				<li><a href="{{ site.baseurl }}/starting/releasing/#changelog">Write useful changelogs</a></li>
				<li><a href="{{ site.baseurl }}/maintaining/github-process/#issue-pr-labels">Triage issues and pull requests</a></li>
				<li><a href="{{ site.baseurl }}/starting/releasing/#security">Handle security responsibly</a></li>
			</ul>
			<div class="path-cta">
				<a href="{{ site.baseurl }}/maintaining/" class="btn-secondary">Explore the full <strong>Maintaining, Supporting, and Enhancing a Project</strong> section »</a>
			</div>
		</div>

		<div class="path-card tertiary">
			<h2>📈 Growing and Sustaining</h2>
			<p>Looking beyond day-to-day maintenance? Scale your project and community:</p>
			<ul>
				<li><a href="{{ site.baseurl }}/growing/#governance">Shape governance</a></li>
				<li><a href="{{ site.baseurl }}/starting/releasing/#credit-management">Build community and recognition</a></li>
			</ul>
			<div class="path-cta">
				<a href="{{ site.baseurl }}/growing/" class="btn-tertiary">Explore the full <strong>Growing and Sustaining a Project</strong> section »</a>
			</div>
		</div>

		<div class="path-card reference">
			<h2>📚 References and Resources</h2>
			<p>Quick access to tools, standards, and examples:</p>
			<ul>
				<li><a href="{{ site.baseurl }}/references/#tools">Tools we recommend</a></li>
				<li><a href="{{ site.baseurl }}/references/#standards">Industry standards</a></li>
				<li><a href="{{ site.baseurl }}/references/#examples">Example repositories</a></li>
			</ul>
			<div class="path-cta">
				<a href="{{ site.baseurl }}/references/" class="btn-reference">See the full <strong>References and Resources</strong> section »</a>
			</div>
		</div>
	</div>

	<div class="intro-section">
		<h2>About This Guide</h2>
		<p>This guide is written with groups releasing smaller-scale open source software in mind. The majority of our open source projects are narrowly-focused extensions to existing ecosystems, such as WordPress plugins or front-end components, and this set of best practices reflects that.</p>
		
		<div class="intro-links">
			<p><strong>New to open source?</strong> <a href="{{ site.baseurl }}#intro">Learn why open source matters</a></p>
			<p><strong>Want to contribute to this guide?</strong> <a href="{{ site.baseurl }}#contributing">See our contributing guidelines</a></p>
		</div>
	</div>
</div>

<div class="docs-section">
	{% capture introduction %}{% include markdown/Introduction.md %}{% endcapture %}
	{{ introduction | markdownify }}
</div>

<style>
.path-cards {
	display: grid;
	grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
	gap: 2rem;
	margin: 2rem 0;
}

.path-card {
	background: #f8f9fa;
	border: 1px solid #e9ecef;
	border-radius: 8px;
	padding: 1.5rem;
	transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.path-card:hover {
	transform: translateY(-2px);
	box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.path-card.primary {
	border-left: 4px solid #007cba;
}

.path-card.secondary {
	border-left: 4px solid #28a745;
}

.path-card.tertiary {
	border-left: 4px solid #ffc107;
}

.path-card.reference {
	border-left: 4px solid #6f42c1;
}

.path-card h2 {
	margin-top: 0;
	margin-bottom: 1rem;
	font-size: 1.25rem;
}

.path-card p {
	color: #6c757d;
	margin-bottom: 1rem;
}

.path-card ul {
	margin-bottom: 1.5rem;
}

.path-card li {
	margin-bottom: 0.5rem;
}

.path-cta {
	text-align: center;
}

.btn-primary, .btn-secondary, .btn-tertiary, .btn-reference {
	display: inline-block;
	padding: 0.75rem 1.5rem;
	border-radius: 4px;
	text-decoration: none;
	font-weight: 600;
	transition: all 0.2s ease;
}

.btn-primary {
	background: #007cba;
	color: white;
}

.btn-primary:hover {
	background: #005a87;
	color: white;
}

.btn-secondary {
	background: #28a745;
	color: white;
}

.btn-secondary:hover {
	background: #1e7e34;
	color: white;
}

.btn-tertiary {
	background: #ffc107;
	color: #212529;
}

.btn-tertiary:hover {
	background: #e0a800;
	color: #212529;
}

.btn-reference {
	background: #6f42c1;
	color: white;
}

.btn-reference:hover {
	background: #5a32a3;
	color: white;
}

.intro-section {
	margin-top: 3rem;
	padding-top: 2rem;
	border-top: 1px solid #e9ecef;
}

.intro-links {
	margin-top: 1rem;
}

.intro-links p {
	margin-bottom: 0.5rem;
}

@media (max-width: 768px) {
	.path-cards {
		grid-template-columns: 1fr;
		gap: 1rem;
	}
	
	.path-card {
		padding: 1rem;
	}
}
</style>