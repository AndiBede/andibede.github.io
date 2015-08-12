---
layout: default
title: Group Members
order: 6
---

<div class="container">
<hr>
<h1>Current group members</h1>
<hr>
 {% assign sorted_pages = site.pages | sort:"order" %}
 {% for page in sorted_pages %}
    {% if page.category == "Members" %}
        <div class="row">
            <div class="col-lg-4">
                <img class ="img-resposiveve" src="/images/{{ page.image }}" height="100" width="100">
            </div>
            <div class="col-lg-8">
            {{ page.content }}
            </div>
        </div>
        <br>
    {% endif %}
{% endfor %}
<hr>
<h1>Former Members</h1>
<hr>
{% for page in sorted_pages %}
    {% if page.category == "Former Members" %}
     <div class="row">
     <div class="col-lg-4">
        <img class ="img-resposiveve" src="/images/{{ page.image }}" height="100" width="100">
    </div>
    <div class="col-lg-8">
        {{ page.content }}
    </div>
    </div>
    <br>
    {% endif %}
{% endfor %}
</div>
