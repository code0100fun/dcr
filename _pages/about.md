---
title: About us
subtitle: We manage a network of global contacts for fuel and other commodities.
description:
featured_image: /images/sunset_oilwells1.jpg
layout: default
---

<section class="hero hero--single">

	<div class="hero__image" style="background-image: url({{ page.featured_image | relative_url }})">
		<div class="hero__overlay"></div>
	</div>

	<div class="wrap">

		<h1>{{ page.title }}</h1>
		<p>{{ page.subtitle }}</p>

	</div>

</section>

<section class="listing">

	<div class="wrap">

		{% for member in site.data.team %}

		<article class="post">

			<div class="post__image-wrap">
				<div class="post__image" style="background-image: url({{ member.image | relative_url }})"></div>
			</div>

			<div class="post__content-wrap">
				<div class="post__content">
					<h2 class="post__title">{{ member.name }}</h2>
					<p class="post__subtitle">{{ member.role }}</p>
					<p class="post__description">{{ member.bio }}</p>
				</div>
			</div>

		</article>

		{% endfor %}

	</div>

</section>