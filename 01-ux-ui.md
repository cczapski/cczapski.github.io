---
layout: page
title: UX / UI
page-title: UX / UI
permalink: /ux-ui/
---

<section class="content work">
	<div class="page">
		{% for page in site.pages %}
		{% if page.id %}
			<a href="{{ page.permalink }}">
				<div id="{{ page.id }}" class="portfolio-image">
					<div class="project-title">
						<h3>{{ page.project }}</h3>
						<p>{{ page.project-brief }}</p>
					</div>
				</div>
			</a>
		{% endif %}
		{% endfor %}
	</div>
</section>


