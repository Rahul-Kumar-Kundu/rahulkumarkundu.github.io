---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order.
nav: true
nav_order: 3
---

{% include bib_search.liquid %}

<div class="publications">

<h2 class="year">Journal Papers</h2>
{% bibliography --query @article %}

<h2 class="year">Conference Proceedings</h2>
{% bibliography --query @inproceedings %}

<h2 class="year">Works in Progress</h2>
{% bibliography --query @unpublished %}

</div>
