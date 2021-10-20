+++
title = "Project Euler"
date = 2010-03-23
+++

I'm a latecomer to the [Project Euler](http://www.projecteuler.net) game, but I'm looking for a strong finish.

I've been trying to hone my Python skills, so I [Dove Into Python](http://www.diveintopython.org) with a vengeance. That didn't quite sate my desire for crazy coding fun, and my good buddy [Sean](http://www.seanyo.ca) suggested the [Infamous FizzBuzz test](http://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/).

Well, I loved it, and I searched for more similar problems, and I got to the first Project Euler question:

> If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Find the sum of all the multiples of 3 or 5 below 1000.

I was thrilled! A minor modification to my fizzbuzz program and I was off and running. I've currently completed somewhere around 20... but I'll admit that I've skipped to the end am trying my hand at Problem 282, the dreaded Ackermann Function.


```python
import itertools
import math
import operator

def ackermann(m, n):
    """This prints out the ackermann number of (m,n) but it's not 
    recommended to try doing more than 4,3."""
    while m >= 4:
        if n == 0:
            n = 1
        else:
            n = ackermann(m, n - 1)
        m -= 1
    if m == 3:
        return (1 << n + 3) - 3
    elif m == 2:
        return (n << 1) + 3
    elif m == 1:
        return n + 2
    else:  # m == 0
        return n + 1


def ackermod(i, j, mod):
    """A modulo Ackermann function"""
    if i == 0:
        return (j + 1) % mod
    if i > 0:
        if j == 0:
            return ackermod(i - 1, j, mod)
        if j > 0:
            return ackermod(i - 1, ackermod(i, j - 1, mod), mod)

```


So - if you're a coder, why don't you try it out?
