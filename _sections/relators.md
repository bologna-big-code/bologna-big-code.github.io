---
title: Relators
order: 4
include: sections/default.html
bg: bg-light 

---

{% assign relators = site.data.relators %}

{% if relators.size > 0 %}
<div class="row">
    <div class="col-4">
        <div class="list-group" id="list-tab" role="tablist">
            {% for relator in relators %}
            <a class="list-group-item list-group-item-action {% if forloop.index==1 %}active{% endif %}" id="{{ relator.name | slugify }}-list" data-bs-toggle="list" href="#{{ relator.name | slugify }}" role="tab" aria-controls="home">{{ relator.name }}</a>
            {% endfor %}
        </div>
    </div>
    <div class="col-8">
        <div class="tab-content" id="nav-tabContent">
            {% for relator in relators %}
            <div class="tab-pane fade show {% if forloop.index==1 %}active{% endif %}" id="{{ relator.name | slugify }}" role="tabpanel" aria-labelledby="{{ relator.name | slugify }}-list">
            <img src="{{ relator.image }}" width="128px" class="rounded float-end">
            {{ relator.desc }}
            </div>
            {% endfor %}
        </div>
    </div>
</div>
{% endif %}