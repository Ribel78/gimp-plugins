# gimp-plugins
Personal Gimp plugins written in Python

<b>Gude Creator</b>

Gudes can be created using selected option from "Add guides from:" menu

"Formula" option:
You can add gudes by describig them using text.
H for horisontal (-) gudes and V for vertical (|) gudes followed by numbers (indegers or floats) describing guide's position starting from the top left corner of the image. Position can be percent or pixels, depending on the toggle "Use percent/pixels"
Example: H25V25H50

Another use of Formula is equidistant guide distribution.
in this case use only letters to indicate the number of guides of different type.
Example: HHHVVVVV

Avoid spaces or other letters in the formula for acurate results.

"Include mirrored guides" toggle can add also guides that are symmetrical to those from the formula.

"Remove previous guides" toggle can clear existing guides before adding the new ones.

The rest of the options use active layer or selection bounds as reference for adding new guides
