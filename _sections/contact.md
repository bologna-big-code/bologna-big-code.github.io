---
title: Contact
order: 6
include: sections/default.html
bg: bg-light

---

<form id="contact-form" name="contact" method="POST" data-netlify="true">
    <div class="form-group">
        <label class="py-2" for="name"><b>Name and surname</b></label>
        <input type="text" name="name" id="name" placeholder="Write your name here" class="form-control">   
    </div>
    <div class="form-group">
        <label class="py-2" for="email"><b>Email</b></label>
        <input type="email" name="email" id="email" autocomplete="email"  class="form-control" placeholder="Write your email here" title="The domain portion of the email address is invalid (the portion after the @)." pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$" required>
    </div>
    <div class="form-group">
        <label class="py-2" for="contest"><b>Contest</b></label>
        <select class="form-select" aria-label="Default select example">
            <option selected>Se partecipi al nostro contest, apri questa sezione</option>
            {% for i in site.data.contest %}
            <option value="{{ i.name | slugify }}">{{ i.name }}</option>
            {% endfor %}
        </select>
    </div>
    <div class="form-group">
        <label class="py-2" for="message"><b>Message</b></label>
        <textarea class="form-control" name="message" id="message" placeholder="Write your message here" rows="7" required></textarea>
    </div>
    <p class="small">By submitting the form contained in this page, you consent to let the organisation collect and store the provided data. 
    You can revoke the consent at any given time and claim the correction or deletion of your personal data.</p>
    <button type="submit" name="submit" class="btn btn-secondary w-100 mt-1 pb-2">Send message</button>
</form>
