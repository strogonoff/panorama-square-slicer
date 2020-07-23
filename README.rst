===============
Panorama slicer
===============

Takes a landscape-oriented image and slices it into even squares with no gap.

Slices are placed in the same directory as input and named
``<your original filename>_slice_<sequential number>.jpg``.

If given horizontally oriented image is not evenly divisible,
fills in the remainder of the last square with white background.

Intermediate output is .tif files, created in the same directory as input.
They are not removed upon completion to avoid data loss.

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

  ./slice <relative/or/absolute/path/to/file.png>
