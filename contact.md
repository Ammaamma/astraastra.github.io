---
layout: page
title: Contact
permalink: /contact/
---

Hi there! Looking to get in touch? Use the contact form below to send me a message.

<form id="contact-form" class="form" action="https://getsimpleform.com/messages?form_api_token=<API-TOKEN>" method="POST" enctype="multipart/form-data">
        <ul class="contact-ul">
            <li class="contact-li">
                <label class="contact-label" for="name">Name:</label>
                <input type="text" placeholder="Enter your name" id="name" class="contact-input" name="name" tabindex="1"/>
            </li>
            <li class="contact-li">
                <label class="contact-label" for="email">Email:</label>
                <input type="email" placeholder="Enter your email" id="email" class="contact-input" name="email" tabindex="2"/>
            </li>         
            <li class="contact-li">
                <label class="contact-label" for="message">Message:</label>
                <textarea class="contact-textarea" placeholder="Your message" class="contact-input" rows="4" id="message" name="message" tabindex="3"></textarea>
            </li>
            
        </ul>
        <input type="submit" value="Send" id="submit"/>
        <input type="hidden" name='redirect_to' value="http://blog.webjeda.com/thank-you/" />
        
</form>



<style>
.contact-li {
    list-style: none;
}

.contact-input {
    border:none;
    border-bottom: 1px solid #eee;
    transition-duration: 0.3s;
    width: 12em;
}

.contact-input:focus {
    outline:none;
    border-bottom: 1px solid {{site.color-1}};
}

.contact-label {
    display: block;
}

ul.contact-ul {
    margin: 0;
    padding: 10px;
}

#submit {
    border:none;
    background-color: {{site.color-1}};
    padding: 5px 15px;
    color: #eee;
    opacity: 0.8;
}

#submit:hover {
    opacity: 1;
    cursor: pointer;
}


#contact-form {
    border: 1px solid #aaa;
    display: inline-flex;
    margin-bottom: 1em;
}

</style>
