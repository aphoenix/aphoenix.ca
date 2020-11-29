+++
title = "How Project Euler got me to Infringe Almost Every Copyright"
date = 2011-03-28
+++

That's a bit of a sensationalist title, but it's also not too far off of true.

I was recently working on a problem for [Project Euler](http://www.projecteuler.net) that starts off like so:

> An irrational decimal fraction is created by concatenating the positive integers:
> 
> 0.123456789101112131415161718192021...

The constructed number is made in such a way that you count from n to infinity, and add whichever number you are on to the decimal expansion. This fraction has several interesting properties. It is normally distributed, but not random. It is a transcendental number, like _pi_ or _e_. It can be constructed in other bases (2, 3, 16) and holds the same properties in those bases. While each of these is mindboggling enough (if you think on them) the thing that drove me to title my post in this way is pretty simple: since this string of numbers contains within it's infinitude every single number that could ever be, and because anything that we have transcribed or copyrighted can be expressed as a sequence of numbers, then _every single copyrighted piece of information in the world is merely a subsection of this string of numbers_.

As an example, let's look at something pretty safe. Here's the first paragraph of the preamble of the [GPL](http://www.gnu.org/licenses/gpl.html):

> The GNU General Public License is a free, copyleft license for software and other kinds of works.

Using a binary encoder, we can see that this text is represented in binary as:

> 01010100 01101000 01100101 00100000 01000111 01001110 01010101 00100000 01000111 01100101 01101110 01100101 01110010 01100001 01101100 00100000 01010000 01110101 01100010 01101100 01101001 01100011 00100000 01001100 01101001 01100011 01100101 01101110 01110011 01100101 00100000 01101001 01110011 00100000 01100001 00100000 01100110 01110010 01100101 01100101 00101100 00100000 01100011 01101111 01110000 01111001 01101100 01100101 01100110 01110100 00100000 01101100 01101001 01100011 01100101 01101110 01110011 01100101 00100000 01100110 01101111 01110010 00100000 01110011 01101111 01100110 01110100 01110111 01100001 01110010 01100101 00100000 01100001 01101110 01100100 00100000 01101111 01110100 01101000 01100101 01110010 00100000 01101011 01101001 01101110 01100100 01110011 00100000 01101111 01100110 00100000 01110111 01101111 01110010 01101011 01110011 00101110

Since this is just a number, it will occur quite naturally somewhere within the string of this constructed decimal. What's even better is _it will occur an infinite amount of times_. This is just a loose and fast example - you could convert this encoding to decimal, and see it again, also an infinite amount of times.

So, if you write a function to express this number, you are, in effect, breaking every restrictive copyright an infinite amount of times. Really, just thinking about this number probably makes a lot of companies gnash their teeth.

By the way, I was not the first to find this or think it interesting. By doing a bit of research, I found out that this number was something called the [Champernowne constant](http://en.wikipedia.org/wiki/Champernowne_constant).

Edit: Also a note: I said "Almost Every Copyright" in my title, because I am neither a Copyright Lawyer or Mathematician.
