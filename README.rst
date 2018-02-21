================================
``mcerp3`` Package Documentation
================================

Overview
========

``mcerp3`` is a stochastic calculator for `Monte Carlo methods`_ that uses 
`latin-hypercube sampling`_ to perform non-order specific 
`error propagation`_ (or uncertainty analysis). 

With this package you can **easily** and **transparently** track the effects
of uncertainty through mathematical calculations. Advanced mathematical 
functions, similar to those in the standard `math`_ module, and statistical
functions like those in the `scipy.stats`_ module, can also be evaluated 
directly.

If you are familiar with Excel-based risk analysis programs like *@Risk*, 
*Crystal Ball*, *ModelRisk*, etc., this package **will work wonders** for you
(and probably even be faster!) and give you more modelling flexibility with 
the powerful Python language. This package also *doesn't cost a penny*, 
compared to those commercial packages which cost *thousands of dollars* for a 
single-seat license. Feel free to copy and redistribute this package as much 
as you desire!

What's New In This Release
==========================

- this is a Python 3 release of the mcerp package by Abraham Lee
  
- officially adds the 3-clause BSD licesnse text to the software
  (this license has been specified in the mcerp PyPI package for years)  


Main Features
=============

1. **Transparent calculations**. **No or little modification** to existing 
   code required.
    
2. Basic `NumPy`_ support without modification. (I haven't done extensive 
   testing, so please let me know if you encounter bugs.)

3. Advanced mathematical functions supported through the ``mcerp.umath`` 
   sub-module. If you think a function is in there, it probably is. If it 
   isn't, please request it!

4. **Easy statistical distribution constructors**. The location, scale, 
   and shape parameters follow the notation in the respective Wikipedia 
   articles and other relevant web pages.

5. **Correlation enforcement** and variable sample visualization capabilities.

6. **Probability calculations** using conventional comparison operators.

7. Advanced Scipy **statistical function compatibility** with package 
   functions. Depending on your version of Scipy, some functions might not
   work.

8. Python 3 support

Installation
============

Required Packages
-----------------

The following packages should be installed automatically (if using ``pip``
or ``easy_install``), otherwise they will need to be installed manually:

- `NumPy`_ : Numeric Python
- `SciPy`_ : Scientific Python
- `Matplotlib`_ : Python plotting library

These packages come standard in *Python(x,y)*, *Spyder*, and other 
scientific computing python bundles.

How to install
--------------

You have **several easy, convenient options** to install the ``mcerp3`` 
package (administrative privileges may be required)

#. Simply copy the unzipped ``mcerp3-XYZ`` directory to any other location that
   python can find it and rename it ``mcerp3``.
    
#. From the command-line, do one of the following:
   
   a. Manually download the package files below, unzip to any directory, and 
      run::
   
       $ [sudo] python setup.py install

   b. If ``setuptools`` is installed, run::

       $ [sudo] easy_install [--upgrade] mcerp3
    
   c. If ``pip`` is installed, run::

       $ [sudo] pip install [--upgrade] mcerp3

See also
========

- `uncertainties`_ : First-order error propagation
- `soerp`_ : Second-order error propagation

Contact
=======

Please send **Python 3 related issues** to `Paul Freeman`_. Other issues should
be referred to the original author, `Abraham Lee`_.


    
.. _Monte Carlo methods: http://en.wikipedia.org/wiki/Monte_Carlo_method
.. _latin-hypercube sampling: http://en.wikipedia.org/wiki/Latin_hypercube_sampling
.. _soerp: http://pypi.python.org/pypi/soerp
.. _error propagation: http://en.wikipedia.org/wiki/Propagation_of_uncertainty
.. _math: http://docs.python.org/library/math.html
.. _NumPy: http://www.numpy.org/
.. _SciPy: http://scipy.org
.. _Matplotlib: http://matplotlib.org/
.. _scipy.stats: http://docs.scipy.org/doc/scipy/reference/stats.html
.. _uncertainties: http://pypi.python.org/pypi/uncertainties
.. _source code: https://github.com/paul-freeman/mcerp
.. _Abraham Lee: mailto:tisimst@gmail.com
.. _Paul Freeman: mailto:paul.freeman.cs@gmail.com
.. _package documentation: http://pythonhosted.org/mcerp3
.. _GitHub: http://github.com/paul-freeman/mcerp
