---
layout: default
title: Group Members
order: 6
---

<div class="container">
<h1>Current group members</h1>
<hr>
 {% assign sorted_pages = site.pages | sort:"order" %}
 {% for page in sorted_pages %}
    {% if page.category == "Members" %}
        <div class="row">
            <div class="col-lg-2">
                <img class ="img-responsive" src="/images/{{ page.image }}" height="100" width="100">
            </div>
            <div class="col-lg-10">
            {{ page.content }}
            </div>
        </div>
        <br>
    {% endif %}
{% endfor %}0px dashed red
<hr>
<h1>Former Members</h1>
<hr>
{% for page in sorted_pages %}
    {% if page.category == "Former Members" %}
     <div class="row">
     <div class="col-lg-2">
        <img class ="img-resposive" src="/images/{{ page.image }}" height="100" width="100">
    </div>
    <div class="col-lg-10">
        {{ page.content }}
    </div>
    </div>
    <br>
    {% endif %}
{% endfor %}
</div>
