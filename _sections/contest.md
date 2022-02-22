---
title: Partecipa al nostro Contest
order: 5
include: sections/default.html
bg: bg-white

---

{% assign list = site.data.contest %}

{% if list.size > 0 %}

<div class="text-center">
    <p>
    Leggi le descrizioni di alcuni dei codici più importanti della storia e scegli quale è il tuo preferito, quale vorresti salvaguardare per i posteri. Spiega la tua motivazione nel form che trovi alla fine della pagina: il commento più curioso e brillante verrà premiato il giorno dell'evento! 
    </p>
    <a data-bs-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample"><i class="bi bi-chevron-double-down"></i></a>
</div>

<div class="pt-3 row collapse" id="collapseExample">
    <div class="col-md-4 mb-5">
        <div class="list-group" id="list-tab" role="tablist">
            {% for i in list %}
            <a class="list-group-item list-group-item-action {% if forloop.index==1 %}active{% endif %}" id="{{ i.name | slugify }}-list" data-bs-toggle="list" href="#{{ i.name | slugify }}" role="tab" aria-controls="home">{{ i.name }}</a>
            {% endfor %}
        </div>
    </div>
    <div class="col-md-8">
        <div class="tab-content" id="nav-tabContent2">
            {% for i in list %}
            <div class="tab-pane fade show {% if forloop.index==1 %}active{% endif %}" id="{{ i.name | slugify }}" role="tabpanel" aria-labelledby="{{ i.name | slugify }}-list">
            {{ i.desc | markdownify }}
            </div>
            {% endfor %}
        </div>
    </div>
</div>
{% endif %}
