+++
title = "Why External Links Should NOT Open in New Tabs"
date = 2012-02-01
+++

I read an article today called [Why External Links Should Open in New Tabs](http://uxmovement.com/navigation/why-external-links-should-open-in-new-tabs/). This is something that is near and dear to my heart, and especially so since it is so very, very wrong.

### Savvy Users have Changed Everything

Users are getting more and more used to how the web works and how to use their browser software. Itâ€™s true that if you ask the average person on the street what a browser is, theyâ€™re likely to say Google, but that doesnâ€™t mean that when they open up â€œthe internetâ€ they donâ€™t know what theyâ€™re doing. Using the web is part of the daily routine for millions of people, and those people are knowing more and more about how to use their browsers. People who know how their browser works know that they have the freedom to open links in another tab.

### What About Old People?

Some people are not frequent users of the internet; they arenâ€™t browser experts. The tabbed interface means nothing to them, and is only a confusion. They look at a browser, and when they click on something, they go somewhere. When they want to get back to where they have been, they use the Back Button. For this reason, opening a new window commits one of the cardinal sins of Usability: **DONâ€™T BREAK THE BACK BUTTON.** I've done UX testing on a good cross section of the population, but my favourite person to test on is my dad. Heâ€™s an "I am not good with computer" sort of person. When a site opens a new window, and he wants to get back to where he was, he cannot get back. He experiences extreme frustration, and stops web browsing. There have been several situations where he has been browsing to make a purchase, gotten frustrated, and left the computer to go to a store in person. That website lost a sale. This is a repeatable pattern; non-savvy person gets frustrated, closes entire window, does not finish call to action.

Iâ€™ve also done UX testing with people who have disabilities. The most frequently checked disability is sight loss; new tabs can present almost insurmountable problems to people who have poor sight. They cause confusion, frustration, and break the fundamental back button. The same is true for people who have cognition issues, or low sight, or manual dexterity issues.

### Back Button Fatigue

This is not a real thing. People understand the back button, and are frustrated when it doesn't work. Savvy users can open in a new window, or use bookmarks for navigation; if they donâ€™t want to use the back button to navigate, they don't.

### Saving Website Resources

This is not an issue for a well crafted website. Your resources should be cached and have proper expires, and will load almost instantly and cost very little overhead after a back press.

### Inaccurate Analytics

This is actually completely backwards. If a user is not _reading_ your site, but has left it to read something else, your analytics should reflect this. They will then return to your site and finish reading. If you use external links, you end up with less useful information about how people are using your site; you over-report the time that people are spending on pages, and do not have an accurate representation of what is happening. Consider these user stories.

Story 1

Dave goes to http://www.acmewidgets.com and starts reading a stellar article about Acmeâ€™s latest widget. After reading for 5 minutes and getting midway through the article, there is a link to a wikipedia page that explains the science behind this widget. Dave opens this link, and it opens in a new tab automatically. Dave reads this page for 15 minutes, then closes that tab. This returns Dave to Acmeâ€™s page, and Dave continues reading for 10 minutes, then closes the Acme Widgets site.

Analytics show: Dave on site for half an hour. Time Dave spent on site: 15 minutes.

#### Story 2

Similar set up. Dave reads the article for 5 minutes, then clicks on a link, which opens in the same tab. He reads that link for 15 minutes, then returns to the site and reads for a further 10 minutes.

Analytics show: Dave on site for 5 minutes, then left, then returned for 10 minutes. Time Dave spent on site: exactly as analytics reported.

Overreporting your analytics is a bad idea. It give you false confidence and decisions based on bad data can give you bad results.

### It's All About Freedom, Baby

The bottom line is this: as a UX designer and developer, you have to consider several different users, and how they can interact with your site. Going out and talking to people about how they interact with a site is very helpful, but itâ€™s even more helpful to observe how people interact with a site, and what causes frustration and what does not. A User should be free to do whatever they want with a given link; open in a new tab, open in the same tab, whatever they want to do. The basic groups to consider here are:

**Super Savvy users, Super Savvy users who are disabled**: theyâ€™re already middle clicking on things they want to open later. Iâ€™m guessing that Anthony, the author, is in this group, because the flow described here is one for a quite savvy user. This group doesnâ€™t care if you open new windows or not, unless you specify to open a new window \*when they want to open the link in the same window\*. Then they experience frustration.

**Medium Savvy users**: they donâ€™t necessarily know to middle click, but they know how to navigate. When something opens in the same tab, they know to use the back button. If something opens in a new tab, they can switch tabs. Theyâ€™ll take whatever you throw at them. They may experience frustration if they click on a link, and have to go back, or re-navigate to your site; this is typically a fairly mild, momentary frustration.

**Medium-Savvy users who are disabled**: New tabs and New windows are _the single worst thing_ on the internet.

**Non-Savvy users, Non-Savvy users who are disabled**: new tabs are scary. The back button is broken. Nothing works the way I want it to work. Iâ€™m closing this whole internet and going to the store or watching TV. New tabs are causing extreme frustration.

### In Conclusion

Making the web accessible should be one of your highest priorities as a UX designer. Everyone needs to be able to do everything on the internet. Itâ€™s not about being fair (though accessibility does aim to be fair); itâ€™s about getting people to do what you want them to do on your website. The bottom line is that making an accessible website isnâ€™t particularly difficult to do, and it will increase your bottom line, whether that is more traffic, more money, or more users.

All links should be left alone to be opened however users want to open them. If you are trying to control how your users experience the web, youâ€™re doing a disservice to them and to your website. Youâ€™ll erroneously inflate some of your analytics, and youâ€™ll frustrate a significant portion of your user base.

_Other resources:_

Nielsen: [http://www.useit.com/alertbox/9605.html](http://www.useit.com/alertbox/9605.html)

Webcredible: [http://www.webcredible.co.uk/user-friendly-resources/web-usability/new-browser-windows.shtml](http://www.webcredible.co.uk/user-friendly-resources/web-usability/new-browser-windows.shtml)
