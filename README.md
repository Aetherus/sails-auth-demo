Auth Demo
=========

Implement Basic Authentication with Sails.js
--------------------------------------------
I know, I know, I am re-invent wheel, for there is already
[Passport][1] and [sails-generate-auth][2].
But because I have a "slightly" different request, and I have 
trouble integrating either into my web app, I decided to
implement it myself.

## Goal
* basic local authentication based on `email` and `password`
* respond with only JSON
* passwords are salted and hashed with `bcrypt` before stored into database
* session-fixation-proof
* send email address validation mails

Let's start.

[1]: https://github.com/jaredhanson/passport
[2]: https://github.com/kasperisager/sails-generate-auth
[3]: https://github.com/plataformatec/devise
