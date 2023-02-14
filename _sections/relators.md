---
title: Relatori
order: 4
include: sections/default.html
bg: bg-light 

---

{% assign relators = site.data.relators %}

{% if relators.size > 0 %}
<div class="row">
    <div class="col-md-4 mb-5">
        <div class="list-group" id="list-tab" role="tablist">
            {% for relator in relators %}
            <a class="list-group-item list-group-item-action {% if forloop.index==1 %}active{% endif %}" id="{{ relator.name | slugify }}-list" data-bs-toggle="list" href="#{{ relator.name | slugify }}" role="tab" aria-controls="home">{{ relator.name }}</a>
            {% endfor %}
        </div>
    </div>
    <div class="col-md-8">
        <div class="tab-content" id="nav-tabContent">
            {% for relator in relators %}
            <div class="tab-pane fade show {% if forloop.index==1 %}active{% endif %}" id="{{ relator.name | slugify }}" role="tabpanel" aria-labelledby="{{ relator.name | slugify }}-list">
                <div class="row">
                    <div class="col-md-12 text-center">
                        <img src="{{ relator.image }}" width="150px" class="rounded-pill border border-5"></div>
                    <div class="col-md-12">
                        {{ relator.desc | markdownify }}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</div>
{% endif %}