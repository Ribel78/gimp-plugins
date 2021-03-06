# gimp-plugins
Gimp plugins written in Python

<h2>Guide Creator</h2>

A plug-in for creating guides based on simple instructions or using active layer or selection as reference.

<h3>Installation:</h3>

Place the <b>guide_creator.py</b> file in <b>\.gimp-2.8\plug-ins\ </b> folder.<br>
In Gimp, the plug-in is located in <b>Image - > Guides -> Guide Creator</b> menu.

<h3>Usage:</h3>

Guides can be created using "Add guides from:" menu.

"Formula" option:

You can add guides by describing them using text description.
H for horisontal (-) guide and V for vertical (|) guide followed by number (indeger or float) describing guide's position starting from the top left corner of the image. Position can be percent of the image width or height or distance in pixels, depending on the toggle "Use percent/pixels".</br>
<b>Example: H25V36.4H50</b><br>
<i>This will add horiszontal guides at 25%( or at 25-th pixel), 50%(or at 50 pixel) along Y axis and a vertical guide at 36.4% (or 36-th pixel) along X axis.</i>


Another use of "Formula" is equidistant guide distribution. In this case use only letters to indicate the number of guides of different type.</br>
<b>Example: HHHVVVVV</b></br>
<i>This will add a 5x3 grid of guides.</i>

Avoid spaces or other letters in the formula for accurate results.

"Include mirrored guides" toggle can add also guides that are symmetrical to those from the formula.

"Remove previous guides" toggle can clear existing guides before adding the new ones.

The rest of the options use active layer or selection bounds as reference for adding new guides.

<h2>Vector To Mask</h2>

A plug-in to convert or update path to layer mask.

<h3>Installation:</h3>

Place the <b>vector2mask.py</b> file in <b>.gimp-2.8\plug-ins\ </b>folder.<br>
In Gimp, right click on active layer and run <b>"Vector to Mask"</b> command.

<h3>Usage:</h3>

The plug-in requires the names of the layer and the path to use as mask to be identical.

Select the layer, right click and choose "Vector to Mask" command.

This will create or update the existing mask for the layer.<br>
The mask is feathered by 2 pixels and can be adjusted additionally with the Levels Tool.<br>
If you don't want this step to be performed comment out the corresponding line in the script.<br>
