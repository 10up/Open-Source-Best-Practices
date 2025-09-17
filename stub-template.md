# Stub Page Template for Open Source Best Practices

This template provides a consistent structure for section landing pages across the Open Source Best Practices site.

## Template Structure

```markdown
---
page: [section-name]
title: [Section Title]
nav: [Navigation Title]
group: navigation
weight: [number]
layout: default
subnav:
  - title: [First Child Page]
    tag: [tag-name]
  - title: [Second Child Page]
    tag: [tag-name]
  - title: [Third Child Page]
    tag: [tag-name]
updated: [date]
---

<div class="docs-section">
	<header>
		<h2>[Section Title]</h2>
		<p>[One-sentence summary for metadata and page description]</p>
	</header>

	<div class="col">
		<h3>Who this is for</h3>
		<ul>
			<li>[Brief description of primary audience]</li>
			<li>[Secondary audience if applicable]</li>
			<li>[Tertiary audience if applicable]</li>
		</ul>
	</div>

	<div class="col">
		<h3>What you'll find here</h3>
		<ul>
			<li>[High-level overview of first type of guide]</li>
			<li>[High-level overview of second type of guide]</li>
			<li>[High-level overview of third type of guide]</li>
			<li>[High-level overview of fourth type of guide]</li>
			<li>[High-level overview of fifth type of guide]</li>
		</ul>
	</div>

	<div class="col">
		<h3>Next steps</h3>
		<p>[Brief introduction to the next steps section]</p>
		<ol>
			<li><a href="{{ site.baseurl }}/[section]/#[page]">[Link to first child page]</a></li>
			<li><a href="{{ site.baseurl }}/[section]/#[page]">[Link to second child page]</a></li>
			<li><a href="{{ site.baseurl }}/[section]/#[page]">[Link to third child page]</a></li>
		</ol>
	</div>
</div>
```

## Usage Guidelines

1. **Replace bracketed placeholders** with actual content
2. **Keep descriptions concise** - aim for 1-2 sentences per bullet point
3. **Use plain language** - avoid jargon when possible
4. **Link to existing content** where available, or create placeholder links for future content
5. **Maintain consistent tone** - helpful, encouraging, and practical

## Section-Specific Notes

- **Starting**: Focus on first-time open source releasers
- **Maintaining**: Target active project maintainers
- **Growing**: Address mature project needs
- **References**: Provide quick access to tools and standards
