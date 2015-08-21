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
					<h3><a href="{{page.permalink}}">{{page.project}}</a></h3>
				</div>
			</div>
			{% endif %}
		{% endfor %}
	</div>
</section>


