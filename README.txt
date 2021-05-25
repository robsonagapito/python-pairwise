====================================
AllPairs test combinations generator 
====================================

AllPairs is an open source test combinations generator written in 
Python, developed and maintained by MetaCommunications Engineering.
The generator allows one to create a set of tests using "pairwise 
combinations" method, reducing a number of combinations of variables
into a lesser set that covers most situations.

For more info on pairwise testing see http://www.pairwise.org.

The easiest way to get started is to check out usage examples in 
the "examples" directory and online at
https://apps.sourceforge.net/trac/allpairs/browser/examples/.


Features
--------

  * Produces good enough dataset.
 
  * Pythonic, iterator-style enumeration interface.

  * Allows to filter out "invalid" combinations during search for the
    next combination.

  * Allows to exclude "previously tested" pairs/combinations.
    
  * Goes beyond pairs! If/when required can generate n-wise
    combinations.


Installation
------------

  To install AllPairs to your Python's site-packages directory, run 
  this command from the command prompt:

    python setup.py install

  Alternatively, you can just copy the entire "pairwise" directory
  somewhere into your Python path.

  Ps.: AllPairs need to run with Python 3

  If you have this problem (windows):

  * ModuleNotFoundError: No module named... *

  You must run this command

  setx PYTHONPATH "<PythonPath>;<PythonPath>\DLLs;<PythonPath>\lib;<PythonPath>\lib\plat-win;<PythonPath>\lib\site-packages"

  Ex.:
  setx PYTHONPATH "C:\Programas\python\3.7.4;C:\Programas\python\3.7.4\DLLs;C:\Programas\python\3.7.4\lib;C:\Programas\python\3.7.4\lib\plat-win;C:\Programas\python\3.7.4\lib\site-packages"

Run
---

  python examples/example1.1.py

Known issues
------------

  * Not optimal - there are tools that can create smaller set covering
    all the pairs. However, they are missing some other important 
    features and/or do not integrate well with Python.
  
  * Lousy written filtering function may lead to full permutation of 
    parameters.
  
  * Version 2.0 has become slower (a side-effect of introducing ability
    to produce n-wise combinations).


Feedback
--------
  
  Please submit patches, bug reports, and feature requests here:
  http://apps.sourceforge.net/trac/allpairs/newticket

  Other inquires can be directed to 
  metacomm(at)users.sourceforge.net
