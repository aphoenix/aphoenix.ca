+++
title = "I am a Page Rank Savant"
date = 2007-07-17
+++

So, try this out, if you're of a mind.

- Go to Google
- Type "Sunny Skies" in the search box
- Search images
- Click on that very first image

You should end up here (or thereabouts): [Sunny Skies](http://www.aphoenix.ca/sunny-skies-10/).

Two questions seem to immediately present themselves now:

**How did I figure that out?** More importantly: **How did I get such a good pagerank?**

Figuring this out was actually pretty easy, but I'll tell you the whole story and, hopefully, give credit where it is due. I was looking through some traffic logs for this site, and noticed something strange. Specifically, there was some traffic coming here from this blog post: [Nothing Good About Summer](http://migraineur.blogspot.com/2007/07/nothing-good-about-summer.html).

"Well, that's weird," thought I. "I wonder what's going on there?" So I went to that post, read it, and saw that the poster is using a photo taken by me in their post. They're mostly complying with my [Creative Commons License](http://www.aphoenix.ca/creative-commons-license/) (a better attribution would be nice, but not necessary), so I certainly don't have a problem with their usage (\[_Edit: Diane has graciously added further attribution to the post and I could not be happier with it!_\]). "But," I wondered. "How did they find the picture?"

I relayed this information to my good friend [Chris](http://blog.ccharles.ca) and he gave me the list of steps above, showing me that my pagerank for "sunny skies" is ~1 for images. That settles that. But how did I get such a good pagerank for this sort of thing?

This is also fairly simple. It's just good coding practices. The post that the image is from contains all the correct meta-information for google to pick it up and categorize it, the image itself is put in properly (with an alt-tag) and I process the site every night with an automatic python script that creates an indexed sitemap.xml that google reads (probably every week or two) and understands. All in all, it's the simplest SEO that one could think about.

I have to say that I love a system that rewards good coding. Thanks Google!
