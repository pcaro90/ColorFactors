Color Factors
=============

Introduction
------------

This small project is the demo submitted to the [JS1K
2013-spring](http://js1k.com/2013-spring/) Competition.

Welcome to Color Factors!
-------------------------

In this world, each point represents a number, starting from 2, to the
infinite. Each one of these number is connected with its factors by an arc. The
colors of the points come from a spring-like rainbow, and the arcs have a
gradient that comes from the colors of the points they are connecting. However,
all primes are white, just because they are cool. The "n" in the top-left
corner indicates the last number, "primes" the number of prime numbers found,
and "last" the last prime number found. If you click anywhere in the screen,
the TURBO MODE will be activated!

Obvious examples:

- 10 is connected with 5, 2, and with its multiples (20, 30, 40...)
- 20 is connected to 10, 5 and 2 (and its multiples)
- 30 is connected to 10, 6, 5, 3 and 2 (and its multiples)
- 31 is only connected with it multiples, because it's prime.

The demo has been tested in OS X, in the following browsers:

- Chrome: Works nicely.
- Safari: Works nicely.
- Firefox: Works, but really slow after a few numbers are added.
- Opera: Works well, after applying a workaround to avoid a fix regarding the
  transformation of arcs.

In order to minify the code, I wrote my own "JSCompressor" in Python, based on
the original [JSCrush by Aivo Paas](http://www.iteral.com/jscrush/), but with
some functionalities that help when trying to find an optimal minimizable code,
obtaining an even more reduced output. Everything else has been done manually,
with some help from my JSCompressor script.

After the compression, the code length is 1019 characters, which is a prime
number. Nice.

_Cool fact_: The obvious property of prime numbers (they don't have factors
besides of 1 and themselves) leads to the fact that they are only connected
with points in their right side, never in their left side.


Names used (and where can that character be found):

 - a: 2d context
 - b: document body
 - c: canvas element
 - C: color function (addColorStop)
 - d: dinc (innerWidth)
 - e: inc (innerHeight)
 - f: ninc (function)
 - g: gradient (innerHeight)
 - h: height (innerWidth)
 - i: loop index (innerWidth)
 - I: list of factors (setInterval)
 - k: loop index (strokeStyle)
 - l: last prime found (fillStyle)
 - n: numbers (innerWidth)
 - p: primes found (addColorStop)
 - r: rinc (innerWidth)
 - S: add_point function (addColorStop)
 - u: movement function (function)
 - v: movement increment
 - w: width (innerWidth)
 - x: aux (fillText)

_Cool fact_: The most used character in this script before compression is "i",
with 74 appearances; followed by "(" and ")", with 73 appearances each; and by
"=" and ";", tied with 59 appearances each (without counting the comments!).

Copyright
---------

Copyright (c) 2013 Pablo Caro. All Rights Reserved.

Pablo Caro <<me@pcaro.es>> - <http://pcaro.es/>
