.. _style_guide:


###########################
Style Guide For Python Code
###########################

************
Introduction
************

******************************************************
A Foolish Consistency is the Hobgoblin of Little Minds
******************************************************

************
Code lay-out
************


Indentation
===========


Tabs or Spaces?
===============


Maximum Line Length
===================



Should a line break before or after a binary operator?
======================================================



Blank Lines
===========



Source File Encoding
====================


Imports
=======



Module level dunder names
=========================


*************
String Quotes
*************


****************************************
Whitespace in Expressions and Statements
****************************************

Pet Peeves
==========

Other Recommendations
=====================


*********
Comments
*********

Block Comments
==============

Inline Comments
===============

Documentation Strings
=====================


******************
Naming Conventions
******************


Overriding Principle
====================

Names that are visible to user as public part of the API should follow conventions that reflect usage rather than implementation.


Descriptive: Naming Styles
==========================

There are a lot off different naming styles. It's helps to recognize what naming style is beening used, independently from what they are used for.
The following naming styles are commonly distinguished:

* ``b`` (single lowercase letter)
* ``B`` (single uppercase letter)
* ``lowercase``
* ``lower_case_with_underscores``
* ``UPPERCASE``
* ``UPDATE_CASE_WITH_UNDERSCORES``
* ``CapitalizedWords`` (**Note**: When using abbreviations in CapWords, capitalize all the letters of the abbreviation. Thus HTTPServerError is better than HttpServerError)
* ``mixedCase`` (differs from CapitalizedWords by initial lowercase character)
* ``Capitalized_Words_width_Underscores`` (**Ugly!**)
* ``_single_leading_underscore``: weak "internal user" indicator. E.g. ``from M import *`` does not import objects whose name start with underscore
* ``single_trailing_underscore``: used by convention to avoid conflicts with Python keywords, e.g::
    
    Tkinter.Toplevel(master, class_='className')

* ``__double_leading_underscores``: when naming a class attribute, invokes name mangling (inside class ``FooBar``,``__boo`` becomes ``_FooBar__boo``)
* ``__double_leading_and_trailing_underscores__``:  "magic" objects or attributes that live in user-controlled namespaces. e.g. ``__init__``, ``__import__`` or ``__file__``. 
  Never invent such names; only use them documented

^^^^^^^^^^^^^^^^^^^^^^^
This is a subsubsection
^^^^^^^^^^^^^^^^^^^^^^^

"""""""""""""""""""
This is a paragraph
"""""""""""""""""""





Prescriptive: Naming Conventions
================================


Names to Avoid
--------------

Never use the characters "l" (lowercase letter el), "O" (uppercase letter oh), "I" (uppercase letter eye) as single character variable names.
In some fonts, these characters are indistinguishable from the numerals one and zero. When tempted to use "l" use "L" instead.

Package and Module Names
------------------------

Modules should have short, all-lowercase names. Underscores can be used in the module name if it improves readability.
Python packages should also have short, all-lowercase names, although the use of underscores is discouraged.
When an extention module written in C or C++ has an accompanying Python module that provides a higher level interface, the C/C++ module has a leading udderscore (e.g. _socket).

Class Names
-----------


Exception Names
---------------


Global Variable Names
---------------------


Function Names
--------------



Function and method arguments
-----------------------------


Method Names and Instance Variables
-----------------------------------


Constants
---------


Designing for inheritance
-------------------------



Public and internal interfaces
==============================

***************************
Programming Recommendations
***************************


Function Annotations
====================

**********
References
**********


*********
Copyright
*********









