===============
Panorama slicer
===============

Takes a landscape-oriented image of 1960px height and arbitrary width.

Slices it into into 1960x1960px squares with no gap.

Slices are placed in the same directory as input and named
``<your original filename>_square_<sequential number>.jpg``.

If landscape is not evenly divisible, fills in the remainder of the last
square with white background.

Intermediate output is .tif files, created in the same directory as input.
They are not removed upon completion to avoid data loss.

.. note:: The image is expected to be 1960px tall.

Use cases
---------

* Instagram carousel.

Pre-requirements
----------------

This is currently a fish script, so that shell must be installed.

It uses ImageMagick’s ``convert`` binary.

Usage
-----

::

  ./slice <path/to/file.png>
