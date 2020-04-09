---
layout: page
title: Publications
permalink: /publications/
---

{% for article in site.data.publications %}
- {{ article.authors }}. *{{ article.title }}*. ***{{ article.journal }}*** ({{ article.year }}) {{ article.pages }}. {% if article.notes %} {{ article.notes }} {% endif %}
{% if article.featured %}
    *Featured in*
	{% for feature in article.featured %}
	- {{ feature }}
	{% endfor %} 
{% endif %}
{% endfor %}


