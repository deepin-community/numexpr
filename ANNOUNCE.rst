========================
Announcing NumExpr 2.7.3
========================

Hi everyone, 

This is a maintenance release to make use of the oldest supported NumPy version 
when building wheels, in an effort to alleviate issues seen on Windows machines 
that do not have the latest Windows MSVC runtime installed. It also adds
wheels built via GitHub Actions for ARMv8 platforms.

Project documentation is available at:

http://numexpr.readthedocs.io/

Changes from 2.7.2 to 2.7.3
---------------------------

- Pinned Numpy versions to minimum supported version in an effort to alleviate 
  issues seen in Windows machines not having the same Windows SDK installed as 
  was used to build the wheels.
- ARMv8 wheels are now available, thanks to `odidev` for the pull request.

What's Numexpr?
---------------

Numexpr is a fast numerical expression evaluator for NumPy.  With it,
expressions that operate on arrays (like "3*a+4*b") are accelerated
and use less memory than doing the same calculation in Python.

It has multi-threaded capabilities, as well as support for Intel's
MKL (Math Kernel Library), which allows an extremely fast evaluation
of transcendental functions (sin, cos, tan, exp, log...) while
squeezing the last drop of performance out of your multi-core
processors.  Look here for a some benchmarks of numexpr using MKL:

https://github.com/pydata/numexpr/wiki/NumexprMKL

Its only dependency is NumPy (MKL is optional), so it works well as an
easy-to-deploy, easy-to-use, computational engine for projects that
don't want to adopt other solutions requiring more heavy dependencies.

Where I can find Numexpr?
-------------------------

The project is hosted at GitHub in:

https://github.com/pydata/numexpr

You can get the packages from PyPI as well (but not for RC releases):

http://pypi.python.org/pypi/numexpr

Documentation is hosted at:

http://numexpr.readthedocs.io/en/latest/

Share your experience
---------------------

Let us know of any bugs, suggestions, gripes, kudos, etc. you may
have.

Enjoy data!


.. Local Variables:
.. mode: rst
.. coding: utf-8
.. fill-column: 70
.. End:
