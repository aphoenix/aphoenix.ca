+++
title = "Guelph Coffee and Code + Project Euler"
date = 2011-03-24
+++

I'm talking about [Project Euler](http://www.projecteuler.net) at tonight's [Guelph Coffee and Code](http://www.guelphcoffeeandcode.org). My talk is going to be short, but here's the main talking points.

### Lenhard Euler: Mathematician

Euler (pronounced "Canada's Worst Hockey Team that's not The Senators") was a Mathematician in the 1700s. He was a genius, and he helped shape the world of mathematics that we know and love today. Check out [Euler on Wikipedia](http://en.wikipedia.org/wiki/Euler) for more in depth info about the fellow.

### What's this all about?

Project Euler is gets you to combine mathematical insights with computer programming in an effort to find answers to a series of over 300 problems. It's not tied to a particular language, though there are some languages that will serve you better than others. It's all about finding the answer in an elegant fashion.

### Why should I care?

Project Euler will help you to identify areas of interest for you, and to make you a better all around programmer (and mathematician). There's a ton of different subjects that are covered, and it's an opportunity to push your self in new directions.

### Let's do an example!

Sure thing! Look at Question #1.

> Add all the natural numbers below one thousand that are multiples of 3 or 5.

Not hard right? Make a loop that goes from 1 to 1000, and for each number check if it's divisible by 3 or divisible by 5. If it is, add it to a running sum. Pseudocode looks something like this:

x=1  
sum=0  
while x is under 1001  
    if x is a multiple of 3 then sum = sum + x  
    if x is a multiple of 5 then sum = sum + x  

And at the end return sum. Does that give the right answer? Are we forgetting something?

Of course, if x is a multiple of both 3 and 5, then we've counted it twice. We can fix that in a few ways, like subtracting off x one time if it's a multiple of 3 and 5.

if x is a multiple of 3 and 5  
then sum = sum - x

Or we could just solve it with an else

if x is a multiple of 3 then sum = sum + xM  
else if x is a multiple of 3 then sum = sum + x

Now a lot of people will understand that the "trick" is not really tricky in this case. Remember not to count multiples of 3 and 5 twice is pretty simple. But the curve is pretty steep - after 20 or 30 questions, it's much more hidden.

And that's the gist of what I'm saying tonight.

By the way, here's that pseudocode in python:

f=0  
x=1  
while x < 1000:  
    if x%3==0:  
        f=f+x  
    elif x%5==0:  
        f=f+x  
    x=x+1  
print f
