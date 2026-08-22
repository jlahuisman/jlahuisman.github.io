---
layout: default
title: Publications
permalink: /publications/
---

<main class="page">
<p class="section-kicker">03 / Publications</p>

<h1>All publications.</h1>

<div class="page-content">

{% assign pubs = site.publications | sort: "year" | reverse %}

{% for pub in pubs %}

<p>
<span class="pub-year">{{ pub.year }}</span>
<br>
<strong>{{ pub.title }}</strong>
<br>
{{ pub.authors }}
<br>
<em>{{ pub.journal }}</em>
</p>
{% endfor %}

</div>
<a class="back" href="{{ '/' | relative_url }}#publications">← Back</a>

</main>
