+++
title = "On Mistakes"
date = 2022-02-04
[taxonomies]
tags = ["reflections", "coding", "leadership"]
+++

About 20 years ago, I worked at The Library for a mid-sized University. I was working on a project that at the time was 
interesting and pushing some technical limitations - the unit I was with had a bunch of resources available as paper, 
and we were using the same source control for paper copies, PDFs, web copies, and were doing the changes between formats 
using XSLT, having stored the data as XML (I know there's better ways to do this now, but this was the late 90s and at 
the time there wasn't). I was doing something with our little service and hit some kind of weird issue - I don't 
remember the specifics of it anymore, but it required changing a setting that I wasn't particularly comfortable doing 
without running it by someone, so I went to a different department and asked the senior developer there what he thought. 
He was pretty busy and didn't think that our project was of particular importance, so he said, "Do whatever the forum 
your on tells you to do, and leave me alone."

So I made a couple of server configuration changes, because that's what I was told to do.

Now, the service I was using was on a machine - an actual physical machine I could go to - which was in a cluster in the 
library, and it also had some other services on it. One notable thing that was on the same physical machine was related 
to checking out books. When I made the changes, they required a reboot, so I did that (as per instructions from senior 
dev) and when things came back, voilà, everything on our site once again worked perfectly. I continued on my little 
project, happy in the knowledge that what I had done worked out with no negative effects.

Outside my office, there was an ever-increasing line of people at the sign-out desk. They were having an issue with 
signing out books; no matter what happened, the sign-out process wasn't being completed. As that line backed up, I had 
another minor question so, being quite oblivious, I went back to the same unit that I talked to before to touch base 
with some other developers. They were freaking out about things, and couldn't help me. Apparently someone had done 
something *somewhere* and people couldn't sign out books! Even worse - the University integrated with other 
Universities' Libraries, and *those* Universities students couldn't sign out books either! There was something 
catastrophic happening!

I, oblivious, just went home.

The next day, I had an email with a meeting notification - I had a meeting at 11 with the senior dev, the director of 
IT, and the CIO of the Library.

The meeting started poorly - the senior developer laid out how I was an idiot, how I took down the machine in question, 
how the source of the issue was my problem. The CIO asked a couple of key questions; "Why did you have access to this? 
Did you talk to someone before doing this?" I answered truthfully; I had been given access by the senior developer,
and I had asked him before doing anything. The CIO was very wise, and instead of berating me, he gently told the senior
developer that not knowing something does not make someone an idiot; were we not, at that moment, in a building
devoted to housing knowledge that most people did not have? Instead, he thought of it as an opportunity for me to learn
about the infrastructure, and suggested that this was a lesson that I would take with me everywhere from now on, and if
I learned from the lesson, then I was not an idiot. He also suggested to the senior developer that *he* was not at
fault either; if the system was such that the senior dev didn't have time to help the junior dev with a question, then
the system was at fault, and by extension, the CIO himself. He asked what could be done to adjust the system so that
things like this would not happen in the future.

In my career, there have been many times I was like the senior developer in this story, but at every point, I try to be
like the CIO, who taught me more about leadership than anyone else.