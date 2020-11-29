+++
title = "Cascading Means Something"
date = 2007-08-29
+++

I had a question from a coworker the other day and it became obvious to me that they did not really understand what the word _Cascading_ meant in the phrase _Cascading Style Sheets_.

Let me 'splain.

No, no. There is too much. Let me sum up.

From the OED defines a Cascade thusly:

> 1\. A waterfall. a. Usually, a small waterfall; esp. one of a series of small falls, formed by water in its descent over rocks, or in the artificial works of the kind introduced in landscape gardening.

At first glance, that might not be particularly helpful, but if you really look at that definition, you'll find that it explains things perfectly. Specifically, I'd like you to think of a series of small falls, and how the first fall _cascades_ over the rest of the falls, and how the falls lower down redirect the water from higher up.

See? It's not a bad analogy.

What happens with CSS is that each definition (or _rock_ in the analogy) directs a particular tag, class, or id (or _water_ in the analogy) to a specific end point. The definitions higher up in the list take effect first, and the definitions lower down in the list take effect after. In a _cascade_ you might say.

Here's an example:

<-- The HTML Code -->
<div id="special" class="interesting">
  <p>Some content</p>
</div>

/\* The CSS \*/
div.special {
  color:#ffffff;
  background-color:#000000;
  }
div#interesting {
  color:#ffff00;
  background-color:#0000ff;
  }

Whatever comes lower in the cascade (the last _rock_ as it were - in this case div#interesting) defines where that bit of water (the div) ends up going. In this case, it's going to be remarkably ugly because #ffff00; and #0000ff; aren't good colour choices, but I think the point is made, and that is this:

Cascading is important - if you're going to be a web developer, I'd suggest learning it.
