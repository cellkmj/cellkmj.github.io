---
layout: page
title: Publications
permalink: /publications/
---

{% for article in site.data.publications %}
- {{ article.authors }}. *{{ article.title }}*. ***{{ article.journal }}*** ({{ article.year }}) {{ article.pages }}. {{ article.notes }}
{% endfor %}


