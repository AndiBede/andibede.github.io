---
layout: default
title: Equipment
order: 2
---

<div class="container">
<h1>The research infrastructure of the NMR laboratory</h1>
<hr>
 {% assign sorted_pages = site.pages | sort:"order" %}
 {% for page in sorted_pages %}
    {% if page.category == "Equipment" %}
        <div class="row">
            <div class="col-lg-6">
                <img class ="img-responsive" src="/images/{{ page.image }}" height="500" width="500">
            </div>
            <div class="col-lg-6">
            {{ page.content }}
            </div>
        </div>
        <br>
    {% endif %}
{% endfor %}
</div>
