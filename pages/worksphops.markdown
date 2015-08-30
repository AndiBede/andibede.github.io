---
layout: default
title: Workshops
order: 6
---
<div class="container">
<h1>The research infrastructure of the NMR laboratory</h1>
<hr>
 {% assign sorted_pages = site.pages | sort:"order" %}
 {% for page in sorted_pages reversed %}
    {% if page.category == "Workshops" %}
        <div class="row">
            <div class="col-lg-3">
                <img class ="img-responsive" src="/images/{{ page.image }}" height="350" width="350">
            </div>
            <div class="col-lg-9">
            {{ page.content }}
            </div>
        </div>
        <br>
    {% endif %}
{% endfor %}
</div>
