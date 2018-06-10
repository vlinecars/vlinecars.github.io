---
layout: page
title: Fleet lists
permalink: /fleetlists/
order: 2
---

Historical fleet lists:

<ul>
{% for post in site.tags.fleetlists %}
  <li>
	<a href="{{ post.url }}">{{ post.date | date: "%B %-d, %Y"  }}</a>
  </li>
{% endfor %}
</ul>

Unfortunately the *V/LineCars.com* team is unable to keep tabs on the changes to V/Line's carriage fleet as actively as we once did.

Any assistance would be much appreciated - contact us at [vlinecars@gmail.com](mailto:vlinecars@gmail.com).