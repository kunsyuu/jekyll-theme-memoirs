---
layout: page
title: Contact
permalink: /contact
comments: false
---
<style type="text/css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.2.1/css/bootstrap.min.css" integrity="sha512-siwe/oXMhSjGCwLn+scraPOWrJxHlUgMBMZXdPe2Tnk3I0x3ESCoLz7WZ5NTH6SZrywMY+PB1cjyqJ5jAluCOg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-icons/1.9.1/font/bootstrap-icons.min.css" integrity="sha512-5PV92qsds/16vyYIJo3T/As4m2d8b6oWYfoqV+vtizRB6KhF1F9kYzWzQmsO6T3z3QG2Xdhrx7FQ+5R1LiQdUA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</style>
<script src="https://challenges.cloudflare.com/turnstile/v0/api.js" defer></script>

<form accept-charset="UTF-8" action="https://formcarry.com/s/BhrVXCNY2Nb" method="POST" enctype="multipart/form-data">
<p class="mb-4">Please send your message to {{site.name}}. I will reply as soon as possible!</p>
<div class="form-group row">
    <div class="col-md-6 mb-3">
        <input class="form-control" type="text" name="name" placeholder="Name*" required>
    </div>
    <div class="col-md-6">
        <input class="form-control" type="email" name="email" placeholder="E-mail Address*" required>
    </div>
</div>
<textarea rows="8" class="form-control mb-3" name="message" placeholder="Message*" required></textarea>
<div class="cf-turnstile" data-sitekey="0x4AAAAAABeAmS509hlZhpGa"></div>
<button class="btn btn-dark" type="submit">Send</button>
</form>
