---
title: Past conferences
nav_order: 5
---

# Past conferences

| Year | Location | Website |
|:-----|:---------|:--------|
{% for c in site.data.conferences -%}
| {{ c.year }} | {{ c.location }} | [ICER {{ c.year }}]({{ c.url }}) |
{% endfor %}

Earlier editions are listed on the [SIGCSE ICER page](https://sigcse.org/).
