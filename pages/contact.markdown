---
layout: default
title : Contact
breadcrumb: Contact
order: 99
---

<!-- Contact Section -->
<section id="contact" class="contact-section">
    <div class="row">
        <div class="col-lg-12">
            <div class="col-lg-12">

                <!-- Form -->
                <form action="https://getsimpleform.com/messages?form_api_token={{ site.simpleform_token }}" method="post" >
                    <div class="col-lg-6 text-left">
                        <div class="form-group">
                            <label for="InputName">Your Name</label>
                            <div class="input-group">
                                <input type="text" class="form-control" name="InputName" id="InputName" placeholder="Enter Name" required>
                                <span class="input-group-addon"><i class="fa fa-asterisk"></i></span></div>
                        </div>
                        <div class="form-group">
                            <label for="InputEmail">Your Email</label>
                            <div class="input-group">
                                <input type="email" class="form-control" id="InputEmail" name="InputEmail" placeholder="Enter Email" required>
                                <span class="input-group-addon"><i class="fa fa-asterisk"></i></span>
                            </div>
                        </div>
                        <div class="form-group">
                            <label for="InputMessage">Message</label>
                            <div class="input-group">
                                <textarea name="InputMessage" id="InputMessage" class="form-control" rows="5" required></textarea>
                                <span class="input-group-addon"><i class="fa fa-asterisk"></i></span>
                            </div>
                            <div class="well well-sm"><strong><i class="fa fa-asterisk"></i> Required Field</strong></div>
                        </div>
                        <input type="submit" name="submit" id="submit" value="Submit" class="btn btn-info pull-center">
                    </div>
                </form>

                <!-- Open Street Map -->
                <div class="col-lg-5 col-md-push-1 well clearfix">
                    <iframe width="425" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://www.openstreetmap.org/export/embed.html?bbox=23.624567091464993%2C46.795557150079745%2C23.6266216635704%2C46.796706630319825&amp;layer=mapnik&amp;marker=46.79613189326907%2C23.6255943775177" style="border: 1px solid black">
                    </iframe>
                    <label class=" text-muted small">B-dul Muncii nr.103-105, cod 400641, Cluj-Napoca, România<br>
                        <a href="http://www.openstreetmap.org/?mlat=46.79613&amp;mlon=23.62559#map=19/46.79613/23.62559" target="_blank">
                            View Larger Map
                        </a>
                    </label>
                </div>
            </div>
        </div>
    </div>
</section>
<script src='https://www.google.com/recaptcha/api.js'></script>
