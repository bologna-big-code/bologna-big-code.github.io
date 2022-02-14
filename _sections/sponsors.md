---
title: About
image: path/to/img
# Set the display order for this section
order: 2
# Specify the layout for this section
include: sections/default.html
# Set style variables
bg-opaque-overlay: rgba(0,200,0,0.3)
bg_image: http://loremflickr.com/2000/600/robot
---

{% assign sponsors = site.data.sponsors %}
<div class="text-center py-4 h3" id="sponsors">
    Sponsors
</div>

{% if sponsors.size > 0 %}
<div class="container text-center" id="sponsors">
    <div class="row">
        {% for sponsor in sponsors %}
        <div class="col">
            <a href="{{ sponsor.link }}" class="text-reset"><img src="{{ sponsor.image }}" height="128" class="d-inline-block align-baseline" alt="" loading="lazy"></a>
        </div>
        {% endfor %}
    </div>
</div>
{% endif %}