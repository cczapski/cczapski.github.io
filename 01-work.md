---
layout: page
title: Work
permalink: /work/
---

<section class="content">
	<div class="page">
		{% for page in site.pages %}
		{% if page.id %}
			<div id="{{page.id}}" class="portfolio-image">
				<div class="project-title">
					<h3>{{page.project-title}}</h3>
					<div class="work-buttons">
						<button class="live"><a href="{{page.live}}">View Live Site</a></button>
						<button class="github"><a href="{{page.github}}">View on GitHub</a></button>
					</div>
				</div>
			</div>
			{% endif %}
		{% endfor %}
	</div>
</section>


