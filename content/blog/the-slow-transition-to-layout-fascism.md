+++
title = "The Slow Transition to Layout Fascism"
date = 2007-08-08
+++

One of the things that I always find important when designing a website is to get rid of as many of the browser specific presets that each browser has as a default style. Think of the page as a whole as a nation and the tags as the individuals - we really should put the layout of the page _as a whole_ above layout of _individuals_. And think of yourself as a little tinpot dictator that has complete and utter control over each and every aspect, except if a client tells you to change something.

To tell the truth, I'm finding it hard to stay with this "fascism" analogy. But I think I've made my point.

You can quash all dissension by resetting all those settings that tend to change browser to browser. It really helps keep things uniform between Firefox and (shudder)IE, or Opera and Konqueror. But what does it do? How does it affect your coding?

First up is the padding / margin bomb. One of the things that is almost always difficult to deal with is the default space in and around objects in different browsers. So I would recommend just getting rid of that space:

\* {
  padding:0;
  margin:0;
  }

Now there are some things that you will have to take into account. Nothing has a default padding or margin anymore. Absolutely nothing. So you'll have to give some things margins and padding according to how you want them to look. There are a few major players to think about.

- <p>
- <ul> or <ol>
- <h\[n\]>

There are others, but these are the ones that will almost _always_ give you a problem if there's no padding or margin. So how to take care of it?

p, ul, ol, h1, h2, h3, h4, h5, h6, pre, label, fieldset {
  margin:1em;
  }

And if you want to get fancy, add this in too:

blockquote {
  margin-top: 1em;
  margin-bottom:1em;
  margin-left:2.5em;
  margin-right:2.5em;
  }

This sets all those most frequently used items to have a standard, fluid margin. Heck, you can leave just this as your website and it wouldn't be terrible as long as your page was well structured and you added a colour and a background colour.

But what does this gain you? Well, developers, it gains you control. If you've ever done anything with a style sheet, you'll know that nailing down those little bugs that exist browser-to-browser can really monopolize your time. This gives you a place to start from that, for the most part, evens out the playing field for the browsers. A little bit of work up front, and you save yourself hours of headache in the end.

And you'll have taken your first step on the road to become a Layout Fascist.
