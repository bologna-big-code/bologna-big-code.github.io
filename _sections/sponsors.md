---
title: Sponsors
order: 2
include: sections/default.html
bg: bg-light

---

{% assign sponsors = site.data.sponsors %}
{% if sponsors.size > 0 %}
<div class="row text-center">
    {% for sponsor in sponsors %}
    <div class="col">
        <a href="{{ sponsor.link }}" class="text-reset"><img src="{{ sponsor.image }}" height="128" class="d-inline-block align-baseline" alt="" loading="lazy"></a>
    </div>
    {% endfor %}
</div>
{% endif %}