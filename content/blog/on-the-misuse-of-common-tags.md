+++
title = "On the Misuse of Common HTML Tags"
date = 2012-04-25
+++

There are a number of HTML tags which are commonly misunderstood and misused. I've done it myself, with some frequency 
over the years. I've argued that some of these are deprecated, when they weren't. And now I've come full circle, and I 
had a full on argument with someone over the use of the `<i>` tag recently, and I wanted to talk about four specific and 
oft misused tags: `<i>`, `<b>`, `<em>`, and `<strong>`.

<!-- more -->

## The Worst Interpretation: `<i>` == `<em>`, `<b>` == `<strong>`

Here is the worst stance you can have.

- `<i>` and `<em>` mean italic and are the same
- `<b>` and `<strong>` mean bold and are the same

There are a lot of people that still think this. It's wrong. These don't have the meanings that you think they do. \<em> 
does not mean italic. `<i>`does not mean italic (not anymore, anyways, though techetymologically that's where it came 
from).

## Better, but not Great: `<i>`-> em, b -> strong

I was in this group for a long time, but after I started reading spec for HTML a few years ago, I started to understand that it's incorrect:

- `<i>`has been deprecated. Always use em instead.
- b has been deprecated. Always use strong instead

Someone told me this and I listened, and went with it. I told other people this for years. I never really stopped to think about too hard, because I figured that better heads than mine had this figured out. The basic argument is that `<i>`and b have no meaning, but em and strong do have meaning. Well, that's crap. They're just tags; they only have the meaning that we attribute to them. Also, if we use this [onto mapping](http://en.wikipedia.org/wiki/Surjective_function), then strong and em have _the exact same problems_ that b and `<i>`do, because they're the same elements. Changing the tag has no added benefit.

## The Right Way: i, b, em, strong are all viable tags

Here's the right answer: i, b, em, and strong are all worthwhile and useful tags to use. That's right - you can use the `<i>`tag and the b tag for things in your code. You're absolutely right to do so! Just understand what each of them mean. Here are my interpretations of the [HTML spec](http://www.w3.org/TR/html5/text-level-semantics.html#the-abbr-element).

### `<i>`

The `<i>`element is for text that is separate from normal prose, using a different voice, but with no particular emphasis. Some valid examples of this are technical jargon, taxonomies, transcriptions of altered states, or (very specifically) ship names in Western texts. These are items which are distinct from things that require emphasis; they are outside of the normal flow, and we do not necessarily want to attribute extra gravity to things inside of `<i>`tags.

For example, _The Edmund Fitzgerald_ gets i-tagged if I were talking about the boat, but if I were talking about the song, I might emphasize _The Wreck of The Edmund Fitzgerald_.

If one were transcribing an experience that one had while under the influence of narcotics, one might put those in italics:


> His eyes adjusted to the dimness after he put down his opium pipe. <i>The walls took a deep breath and expelled it 
> slowly</i>. "This," thought the man, "is very good." 


If one were to explain in writing to the captain, via blog post, that one was out of <i>dilithium crystals</i> for the 
<i>warp drive</i>, one could use an `<i>` tag.

### b

This is for use similarly; ascribing no extra emphasis, but without the need for a different voice. The best example for this is straight from the spec: text-driven adventure games where items are denoted, but have no particular emphasis on the items:

> You enter a small room. Your sword glows brighter. A rat scurries past the corner wall. 


### em

Semantic markup for text _that is emphasized_ for whatever reason - it attributes greater gravity to that section of the text.

>  You use this tag whenever <em>something</em> is quite important.

### strong

Semantic markup for text **with strong emphasis**. This is text that has the greatest gravity.

> Use this to <strong>emphasize</strong> things, not just to make them bold.


And that is probably more discussion that you've ever cared to read on those particular HTML tags!
