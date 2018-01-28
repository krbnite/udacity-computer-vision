We'll be going over Account Kit, Facebook Login, and the Graph API.

This course is about making the login experience smooth and simple: no password!  Maybe if
I create some kind of App, we can implement this for our automations...

We'll be looking at the Facebook authorization flow... Traditional sign-in and password flow
is slow and fraught w/ security issues. This passwordless login technique is Facebook's 
solution; it ensures customer engagement is not hindered by failed logins. "As a developer,
you should do everything you can to ensure your users can access your app."

## Why use Facebook's Passwordless Login
People forget their passwords all the time.  They quote a statistic on this, which basically
goes like this: If your user forgets their password, they stop giving fux about your app.  Another
concern is typing in the wrong user name or password: fux are diminished quite a bit at the 
error screen.

Fact is, you want your user to give a full dose of fux to your app!

The #1 reason to use a passwordless login solution is convenience for your users.  Just so happens
that better control and security comes along with the package!

## Account Kit
Account Kit allows users to login with their phone number or email address, and authenticate their
identity with no password and no Facebook account.

## Facebook Login
Facebook Login allows users to login with the click of a button, and authenticate their identity using
their Facebook credentials.  Facebook Login has been helping companies use passwordless login in their apps
since 2009. Apparently, it helped to increase signups and retention for many of the companies that used
it.  If a user permits it, you can access their Facebook data through the Graph API (can help to customize
their experience on your app).

## So, wait -- why do we need Account Kit if Facebook Login already works so well?!
Simple: not everyone has a Facebook account. Furthermore, not everyone with a Facebook account wants your
app associated with their Facebook account.

