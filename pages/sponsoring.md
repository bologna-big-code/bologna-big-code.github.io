---
layout: page
title: Sponsoring
permalink: /sponsoring
section: sponsoring

---

The Bologna Federated Conference on Programming Language (BOPL) 2020 includes four conferences on software programming:

- 28th International Workshop on Functional and Logic Programming;
- 30th International Symposium on Logic-Based Program Synthesis and Transformation;
- 3rd International Conference on Microservices;
- 22nd International Symposium on Principles and Practice of Declarative Programming.

Besides **programming languages**, the international community behind BOPL spans areas of computer science that include
**software engineering**, **artificial intelligence**, **security**, **logics**, and **mathematics** and it brings together *200+
researchers and practitioners* to present the latest developments in their respective fields.

**BOPL 2020 [welcomes corporate donations](#supporting-bopl-2020)** to help maintain and improve the overall experience
of attending the conference. We will use money from corporate sponsors to subsidise attendance, especially for students
(e.g., with prizes in dedicated sessions), and to cover the costs of the organisation and of the fees to let the
contents of BOPL be open access to everyone.

<div class="py-4 h3">BOPL 2020 Sponsors</div>

{% include page-sidebar.html %}

<!-- <div id="supporting-bopl-2020" class="py-4 h2">Sponsoring BOPL 2020</div> -->

<div id="supporting-bopl-2020" class="py-4 h3">
	BOPL 2020 Support tiers
</div>

<div class="alert alert-info font-weight-bold text-center" role="alert">
  The deadline to respond to the BOPL 2020 Call for Sponsors is July 17th, 2020.
</div>

BOPL welcomes corporate donations. To help donors orient on their decision, we include below a set of suggested tiers,
donation quotas, and related benefits &mdash; <i>tiers are clickable and direct you to the contact [form for donations](#become-sponsor) at the end of this page</i>.

<div class="card tierLink-bronze mt-3">
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header" style="background-color:#f4a460;">
			Bronze
		</div>
	</a>
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header">
			Suggested donation <strong>250€</strong>
		</div>
	</a>
	<div class="card-body">
		<strong>Benefits:</strong>
		<ul>
			<li>your name and logo prominently displayed on the BOPL website.</li>
		</ul>
	</div>
</div>

<div class="card tierLink-silver mt-2">
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header" style="background-color:#c0c0c0;">Silver</div>
	</a>
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header">
			Suggested donation <strong>500€</strong>
		</div>
	</a>
	<div class="card-body">
		<strong>Benefits:</strong>
		<ul>
			<li>the benefits of the Bronze tier;</li>
			<li>the opportunity to give a 30-minute talk at a joint session with all the attendees of the four
				conferences.</li>
		</ul>
	</div>
</div>

<div class="card tierLink-gold mt-2">
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header" style="background-color:#ffd700;">
			Gold
		</div>
	</a>
	<a href="#become-sponsor" class="text-reset">
		<div class="card-header">
			Suggested donation <strong>1000€</strong>
		</div>
	</a>
	<div class="card-body">
		<strong>Benefits:</strong>
		<ul>
			<li>the benefits of the Silver tier (they include also those of the Bronze tier);</li>
			<li>acknowledgement as a sponsor of the joint sessions of the four conferences keynote talks;</li>
			<li>your name and logo prominently displayed on the video stream at the beginning and ending of each session
				of all conferences (usually there are 5 or 6 sessions a day per conference);</li>
			<li>other arrangements are possible based on your needs and interests.</li>
		</ul>
	</div>
</div>

<div id="become-sponsor" class="py-4 h3">
	Becoming a BOPL 2020 Sponsor
</div>

You can make a donation to BOPL 2020 and become one of its sponsors by contacting the Financial Chair directly (<a
	href="mailto:saverio.giallorenzo@gmail.com?subject=Sponsoring%20BOPL%202020" target="_blank"
	class="btn btn-info btn-sm">Saverio Giallorenzo</a>) or by submitting the form below, reporting your preferred
options, so that we can contact you back.

<form id="fs-frm" name="sponsing-contact-form" accept-charset="utf-8"
	action="https://formspree.io/saverio.giallorenzo@gmail.com" method="post">
	<div class="form-group">
		<label for="name">Contact name</label>
		<input type="text" class="form-control" id="name" name="contact" placeholder="Your name">
		<label class="mt-2" for="email">Contact email</label>
		<input type="email" class="form-control" id="email" aria-describedby="emailHelp" name="email"
			placeholder="Your email">
		<small id="emailHelp" class="form-text text-muted">Your name and email will only be used for the purpose of
			contacting you back and it will not be shared with anyone else.</small>
		<div class="mt-2"></div>
		<label for="exampleInputEmail1">Sponsoring tier your are interested in:</label>
		<div></div>
		<div class="form-check form-check-inline">
			<input class="form-check-input" type="radio" name="tierOption" id="bronze" value="bronze" checked>
			<label class="form-check-label" for="bronze">Bronze</label>
		</div>
		<div class="form-check form-check-inline">
			<input class="form-check-input" type="radio" name="tierOption" id="silver" value="silver">
			<label class="form-check-label" for="silver">Silver</label>
		</div>
		<div class="form-check form-check-inline">
			<input class="form-check-input" type="radio" name="tierOption" id="gold" value="gold">
			<label class="form-check-label" for="gold">Gold</label>
		</div>
	</div>
	<div class="form-group">
		<label for="notes">Additional notes</label>
		<textarea class="form-control" id="notes" name="notes" rows="3"></textarea>
		<small id="emailHelp" class="form-text text-muted">Feel free to use the space above to include or request any additional
			information regarding the sponsorship.</small>
	</div>
	<button type="submit" name="submit" class="btn btn-primary w-100 p-3">Submit</button>
</form>

<script>
	$(".tierLink-bronze").click(function () {
		$("#bronze").trigger("click");
	});
	$(".tierLink-silver").click(function () {
		$("#silver").trigger("click");
	});
	$(".tierLink-gold").click(function () {
		$("#gold").trigger("click");
	});
</script>