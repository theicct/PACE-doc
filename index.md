---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: PACE Model Documentation
---

The ICCT’s PACE model is a global aviation emissions model. The PACE model is intended to help policymakers worldwide to identify and understand trends in the aviation sector, assess emission impacts of different policy options, and frame plans to effectively reduce emissions of both greenhouse gases (GHGs) and local air pollutants. It is designed to allow transparent, customizable estimation of aviation emissions for a broad range of policy cases.

## Versions

PACE is under continuing development. Documentation of all versions since v1.0 can be found here.

{% assign pages = site.pages | sort: "title" | reverse %}
{% for page in pages %}
{% if page.dir contains '/versions/' and page.title contains 'PACE v'%}
<li><a class="page-link" href="{{ page.url | relative_url }}">{{ page.title | escape }}</a></li>
{% endif %}
{% endfor %}
