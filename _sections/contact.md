---
title: About
image: path/to/img
# Set the display order for this section
order: 5
# Specify the layout for this section
include: sections/default.html
# Set style variables
bg-opaque-overlay: rgba(0,200,0,0.3)
bg_image: http://loremflickr.com/2000/600/robot
---

<div class="text-center py-4 h3" id="contact">
    Contact
</div>

<form id="contact-form" name="contact" method="POST" data-netlify="true">
    <!-- <div class="form-group">
        <label for="name"><b>Name</b></label>
        <input class="form-control" type="text" name="name" id="name" autocomplete="name" placeholder="Your name" title="Please enter your name" required>
    </div> -->
    <div class="form-group">
        <label for="email"><b>Email</b></label>
        <input class="form-control" type="email" name="email" id="email" autocomplete="email" placeholder="Your email address" title="The domain portion of the email address is invalid (the portion after the @)." pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$"
            required>
    </div>
    <!-- <div class="form-group">
    <label for="phone"><b>Phone</b></label>
    <input class="form-control" type="text" name="phone" id="phone" autocomplete="tel-national"
      placeholder="A contact number, optional">
  </div> -->
    <div class="form-group">
        <label for="message"><b>Message</b></label>
        <textarea class="form-control" name="message" id="message" placeholder="Write your message here" rows="7" required></textarea>
    </div>
    <button type="submit" name="submit" class="btn btn-secondary w-100 mt-2 p-2">Submit</button>
</form>