Context
-------
Seminar given at the Korea Advanced Institute of Science and Technology

Title:

Eff-Bayes: modular implementations of approximate Bayesian inference
with effect handlers

Abstract:

 I will describe work-in-progress, implementing a library for Bayesian
 inference algorithms for statistical probabilistic programming in the
 programming language Eff using algebraic effects and handlers. During
 the demonstration, I will introduce both programming with effects
 handlers and probabilistic programming.

Joint work with Matija Pretnar, Žiga Lukšič, Oliver Goldstein, and Adam Ścibior.


Installation
------------

You will need a version of Eff with basic support for file output:

    git clone https://github.com/ohad/eff.git
    cd eff
    git checkout eff-spls-2019

and then build this eff:

    opam   install .
or
    opam reinstall .


Usage
-----

Best viewed in an emacs editor split three-ways:

     +------------------------------------------------+-------------------
     |                                                |                  |
     |                                                |                  |
     |   kaist-demo.eff                               |  <shell2>        |
     |                                                |                  |
     |                                                |                  |
     |                                                |                  |
     |                                                |                  |
     |                                                |                  |
     |                                                |                  |
     |------------------------------------------------+                  |
     |    <<shell1>                                   |                  |
     +-------------------------------------------------------------------+


resised so that the .eff buffer's top and bottom rows contain the asterisks.

Is you 'I-search' for '(**********************************' and hit
return, you will be able to or 'I-search' and 'I-search backward' for
the next/previous slide.

In <<shell1>> navigate to the current directory.
In <<shell2>> 'make eff' which will load the definitions into eff
Start the slides
In slides that call the 'plot' function, use 'make' to generate the
appropriate plot, in this order:

    make plot
    make prior_regression
    make silly_regression
    make importance_regression
    make smc_regression



If you have any questions, email <ohad.kammar@ed.ac.uk>

Enjoy!
