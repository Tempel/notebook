A pocket notebook
=================

These are design files for a pocket notebook, designed to hold a pad of sticky
notes, a pen, and small scraps of paper.  It is designed to be made primarily
from leather and wood, using rivets to hold it together, and a snap to hold it
closed.


Files
-----

FreeCAD was used to create the overall geometries.  These were exported as SVG
files and hand modified in Inkscape to create the inputs to the laser cutter.

* _lengths.fcstd_: A top-down layout of the closed notebook, containing a full
  pad of sticky notes, both backing plates, and the leather exterior.
* _notebook.fcstd_: Layout of all parts for laser cutting.  Positioned as if
  the notepad was lying face-down on a table, with the leather exterior on top.
  The drawing view is exported as an SVG for editing in Inkscape.
* _leather.svg_ & _leather.ngc_: Toolpath and G-code for cutting the leather
  backing.  Converted to paths, split into layers, and exported with a feed
  rate of 350 mm/minute.
