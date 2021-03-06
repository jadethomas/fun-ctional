# `curry`

[home](../README.md) &gt; [`curry`](http://ramdajs.com/docs/#curry)

From the Ramda documentation:

> Returns a curried equivalent of the provided function. The curried function has two unusual capabilities. First, its arguments needn't be provided one at a time. If f is a ternary function and g is R.curry(f), the following are equivalent:

    - g(1)(2)(3)
    - g(1)(2, 3)
    - g(1, 2)(3)
    - g(1, 2, 3)

Ramda also has a special placeholder function, `__`:

> Secondly, the special placeholder value `__` may be used to specify "gaps", allowing partial application of any combination of arguments, regardless of their positions. If g is as above and _ is `__`, the following are equivalent:

    - g(1, 2, 3)
    - g(_, 2, 3)(1)
    - g(_, _, 3)(1)(2)
    - g(_, _, 3)(1, 2)
    - g(_, 2)(1)(3)
    - g(_, 2)(1, 3)
    - g(_, 2)(_, 3)(1)

This one is pretty tricky.

[Solutions](./solutions.md)
