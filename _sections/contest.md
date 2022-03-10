---
title: Partecipa al nostro Contest
order: 6
include: sections/default.html
bg: bg-light

---

{% assign list = site.data.contest %}

{% if list.size > 0 %}

<div class="text-center">
    <p>
    Leggi le descrizioni di alcuni dei codici più importanti della storia e scegli quale è il tuo preferito, quale vorresti salvaguardare per i posteri. Motiva la tua scelta nel form che trovi alla fine della sezione: il commento più curioso e brillante verrà premiato il giorno dell'evento! 
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
    <br />
    <form id="contest-form" name="contest" method="POST" data-netlify="true">
        <div class="form-group">
            <label class="py-2" for="name"><b>Nome e Cognome</b></label>
            <input type="text" name="name" id="name" placeholder="Scrivi qui il tuo nome" class="form-control">   
        </div>
        <div class="form-group">
            <label class="py-2" for="email"><b>Email</b></label>
            <input type="email" name="email" id="email" autocomplete="email"  class="form-control" placeholder="Scrivi qui la tua email" title="The domain portion of the email address is invalid (the portion after the @)." pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$" required>
        </div>
        <div class="form-group">
            <label class="py-2" for="contest"><b>Contest</b></label>
            <select name="code[]" class="form-select" aria-label="Default select example" multiple>
                <option selected>Scegli qui il codice che vuoi selezionare</option>
                {% for i in site.data.contest %}
                <option value="{{ i.name | slugify }}">{{ i.name }}</option>
                {% endfor %}
            </select>
        </div>
        <div class="form-group">
            <label class="py-2" for="message"><b>Messaggio</b></label>
            <textarea class="form-control" name="message" id="message" placeholder="Scrivi qui la tua motivazione o un tuo commento" rows="7" required></textarea>
        </div>
        <button type="submit" name="submit" class="btn btn-secondary w-100 mt-2 pb-2">Invia la tua risposta</button>
    </form>

</div>
{% endif %}
