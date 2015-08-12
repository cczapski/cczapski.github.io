---
layout: page
title: Work
permalink: /work/
---

<section class="content">
	<div class="page">
		<a href="portfolio.html"><h2 id="portfolio">Portfolio</h2></a>
		{% for page in site.pages %}
		{% if page.id %}
			<div id="{{page.id}}" class="portfolio-image">
				<div class="project-title">
					<h3>{{page.project-title}}</h3>
				</div>
			</div>
			{% endif %}
		{% endfor %}
	</div>
</section>


