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
* _notebook.fcstd_: Layout of all parts for laser cutting.  Positioned in the
  model as if the notepad was lying face-down on a table, with the leather
  exterior on top, but flipped (leather exterior on bottom) in the drawing
  view.  The drawing view is exported as an SVG for editing in Inkscape.
* _all.svg_: Export of the drawing view from notebook.fcstd, containing all
  parts in final arrangements.  Imported into a new file (the G-code exporter
  didn't like the straight export), edited to have borders of the laser bed
  size (9" x 13"), ungrouped and converted circles to paths, then copied to
  make paths for each part individually.
* _leather.svg_ & _leather.ngc_: Toolpath and G-code for cutting the leather
  backing.  Converted to paths, split into layers, and exported with a feed
  rate of 350 mm/minute.
* _backing.svg_ & _backing.ngc_ and _pocket.svg_ & _pocket.ngc_: Toolpath and
  G-code for cutting the major wooden components.  Converted to paths, split
  into layers, and exported with a feed rate of 300 mm/min.
* _border.svg_ & _border.ngc_: Toolpath and G-code for cutting the notepad
  border pieces.  Also made out of wood, with the same feed rate, but four of
  these pieces must be cut to make a notebook, whereas only one of each other
  piece is needed.


License
-------

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
