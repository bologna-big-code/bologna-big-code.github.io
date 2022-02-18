---
title: Contest
order: 5
include: sections/default.html
bg: bg-white

---

{% assign contest = site.data.contest %}

{% if contest.size > 0 %}
<div class="row">
    <div class="col-4">
        <div class="list-group" id="list-tab" role="tablist">
            {% for scheda in contest %}
            <a class="list-group-item list-group-item-action {% if forloop.index==1 %}active{% endif %}" id="{{ scheda.name | slugify }}-list" data-bs-toggle="list" href="#{{ scheda.name | slugify }}" role="tab" aria-controls="home">{{ scheda.name }}</a>
            {% endfor %}
        </div>
    </div>
    <div class="col-8">
        <div class="tab-content" id="nav-tabContent">
            {% for scheda in contest %}
            <div class="tab-pane fade show {% if forloop.index==1 %}active{% endif %}" id="{{ scheda.name | slugify }}" role="tabpanel" aria-labelledby="{{ scheda.name | slugify }}-list">
            <img src="{{ scheda.image }}" width="128px" class="rounded float-end">
            {{ scheda.desc }}
            </div>
            {% endfor %}
        </div>
    </div>
</div>
{% endif %}

By submitting the form contained in this page, you consent to let the organisation collect and store the provided data. 
You can revoke the consent at any given time and claim the correction or deletion of your personal data.

<form id="contact-form" name="contact" method="POST" data-netlify="true">
    <div class="form-group">
        <label for="email"><b>Email</b></label>
        <input class="form-control" type="email" name="email" id="email" autocomplete="email" placeholder="Your email address" title="The domain portion of the email address is invalid (the portion after the @)." pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$"
            required>
    </div>
    <div class="form-group">
        <label for="message"><b>Message</b></label>
        <textarea class="form-control" name="message" id="message" placeholder="Write your message here" rows="7" required></textarea>
    </div>
    <button type="submit" name="submit" class="btn btn-secondary w-100 mt-2 p-2">Submit</button>
</form>