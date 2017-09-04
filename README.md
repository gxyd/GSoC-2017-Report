# GSoC 2017 Final Submission

This year’s chapter of Google Summer of Code is ending on 29th August 2017. I worked on symbolic integration this time. Below is a mention of the work that was done and the work that remains to be done.

Unmerged Pull Requests
======================

* Make DifferentialExtension object immutable [#12752](https://github.com/sympy/sympy/pull/12752)
* Parametric Logarithmic Derivative: using Risch structure Theorem [#12885](https://github.com/sympy/sympy/pull/12885)
* Implementation of DifferentialExtension for 'tan' [#13095](https://github.com/sympy/sympy/pull/13095)

Merged Pull Requests
====================

* Add repr() printing & dummy=False for DifferentialExtension object [#12372](https://github.com/sympy/sympy/pull/12372)
* Add test for a case in prde_no_cancel_b_large [#12659](https://github.com/sympy/sympy/pull/12659)
* `PolyMatrix` class for a matrix of polynomials [#12694](https://github.com/sympy/sympy/pull/12694)
* Change printing of DifferentialExtesion object, add `__eq__` [#12727](https://github.com/sympy/sympy/pull/12727)
* Change 'Matrix' to 'PolyMatrix' in prde.py and its test file [#12734](https://github.com/sympy/sympy/pull/12734)
* Liouvillian cases for Parametric Risch differential equation [#12743](https://github.com/sympy/sympy/pull/12743)
* separate rewrite functions of exps/pows and logs from `__init__` [#12849](https://github.com/sympy/sympy/pull/12849)
* Add new variables for trigonometric and algebraic extensions [#12850](https://github.com/sympy/sympy/pull/12850)
* Fix (pi\*\*3).is_algebraic in the `_eval_algebraic` in Pow [#12924](https://github.com/sympy/sympy/pull/12924)
* Expression having "I"(iota) be rewritten in terms of 'exp'/'log' in DifferentialExtension[#13225](https://github.com/sympy/sympy/pull/13225)

We touched some part of trigonometric function integration, it wouldn't be wrong to say that trigonometric function integration hasn't been improved much (leave the part of touching the algebraic function integration).

What should be done is to first complete the pull request on differential extesnion construction of trigonometric functions, i.e 'sin', 'cos', etc. There were also two papers which I studied during the GSoC period but didn't implement them, the first being the paper by [Jeffrey and Rich](http://www.apmaths.uwo.ca/~djeffrey/Offprints/toms1994.ps), it isn't embeded in the Risch algorithm but rather use it as a last postprocessing step.

The other important paper being the "Simplification of Real Elementary functions" (isn't publicily available), which I did read but could implement, that is related to the Risch structure theorem's.

Personally, I hoped I could have done better.

Regards,

Gaurav Dhingra
