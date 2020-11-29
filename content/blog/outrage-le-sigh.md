+++
title = "Wordpress Scandal! Outrage!"
date = 2009-05-28
+++

I'm a Wordpress fan, it's true. There, you've got full disclosure\*.

I just finished reading [a ridiculous article on how not to do web site user registration](http://appsecstreetfighter.com/2009/05/23/how-not-to-do-web-site-user-registrationndl/). Read the article - are you outraged at Wordpress now? Well, you should be until you learn how Wordpress stores passwords.

Wordpress stores your password in the "users" table of your database, and here's a surprise - it's a hash (if you know not of the hashes, then I suggest either googling it or just forgetting about this article - it might not be worth your time). Has the crack Wordpress team figured out how to crack hashes? Are they hacking into everything _right now_?

The answer, of course, is no. What happens when you register for a Wordpress site is actually very reasonable. They generate a password randomly. They put that password in an email to you. They work the hash voodoo on it and put it in the database, where it is absolutely not stored in plain text.

The alarmist backlash article is a ridiculous knee-jerk reaction. The problem, obviously is the fact that the email does not insist that you change your password, and that people would even _consider_ keeping a password that is randomly generated for them. My favourite thing about the whole post is that the people who wrote it are a Software Security Institute. I'll accept that one can make mistakes - perhaps a retraction is in order?

\* - actually, I'm also a Drupal guy. And you thought never the twain should meet!
