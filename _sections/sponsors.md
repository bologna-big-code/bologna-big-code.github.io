---
title: Promotori
order: 2
include: sections/default.html
bg: bg-light

---

{% assign sponsors = site.data.sponsors %}
{% if sponsors.size > 0 %}
<div class="row text-center">
    {% for sponsor in sponsors %}
    <div class="col-sm p-1" style="height: 128px">
        <a href="{{ sponsor.link }}" class="text-reset"><img src="{{ sponsor.image }}" class="d-inline-block align-baseline mh-100 mw-100" alt="" loading="lazy"></a>
    </div>
    {% endfor %}
</div>
{% endif %}