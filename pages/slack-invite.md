---
layout: page
title: Request Invite to Slack Team
permalink: /slack-invite
section: slack-invite

---

Please use this form to request an invitation to the BOPL 2020 Slack workspace. Enter the email address that you used when you registered for BOPL.

The Slack workspace is where you will receive instructions on how to access the conference content, and it is where all discussions of all the BOPL conferences and Q&A will take place.

IMPORTANT: Please use your full name when you accept the Slack invitation. At a physical conference you would have a name badge, and at our virtual conference it is important to replicate this so that all conference attendees know with whom they are communicating.

<form id="slack-form" name="slack" method="POST" data-netlify="true">
    <div class="form-group">
        <label for="email"><b>Email</b></label>
        <input class="form-control" type="email" name="email" id="email" autocomplete="email"
            placeholder="Your email address"
            title="The domain portion of the email address is invalid (the portion after the @)."
            pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$"
            required>
    </div>
    <div class="form-group">
        <label for="conference"><b>Conference</b></label>
        <select class="form-control" id="conference">
        <option>28th International Workshop on Functional and Logic Programming</option>
        <option>30th International Symposium on Logic-Based Program Synthesis and Transformation</option>
        <option>3rd International Conference on Microservices 2020</option>
        <option>22nd International Symposium on Principles and Practice of Declarative Programming</option>
        </select>
    </div>
    <button type="submit" name="submit" class="btn btn-primary w-100 p-3">Request Slack Invitation</button>
</form>