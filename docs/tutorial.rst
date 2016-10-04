.. _ShortTutorial:

==============
Short Tutorial
==============

This is a short tutorial that takes you on a tour of some of the more important
features of Imspector. If this is the first time you use the program, it is a good idea
to follow it step by step using the test data that should have been provided to you
with the program.


Getting Started
----------------

.. _ConfigDir:

The Configuration Directory
----------------------------

Loading Data
----------------------------

Displaying Data
----------------------------

Magnifying Glass
******************

If you hold down the Shift key and drag with the left mouse button in a window a magnifying glass is displayed. Shift+Alt keys display an even bigger magnifying glass.

When you are pressing the shift key AFTER starting to drag it will force a vertical or horizontal line when selecting a line profile.

Shortcuts
*********

F9/F10 Fit maximum/minimum.
In a stack view this adjusts the colormap max/min to the maximum/minimum of the current selection, in a graph view the y-axis scale to the maximum/minimum value between the slider bars.

Pg Up/Down Go up/down one slice along the z-axis.
Also pressing the Shift key moves 10, pressing Shift+Alt moves 100 slices along the z-axis.

Ctrl+Pg Up/Down Go up/down one layer along the hidden axis.
Also pressing the Shift key moves 10, pressing Shift+Alt moves 100 layers along the hidden axis. 

Color Maps
----------------------------

Graphs
----------------------------

Drag, Drop, Cut and Paste
----------------------------

Graphs, image stacks and colormaps can be dragged and dropped between windows. This is done by pressing the Ctrl key while dragging with the left mouse button. Colormaps can be dragged onto stacks which will then be displayed using the dropped colormap. For data the following rules apply
Ctrl: Copy all slices of the current selection to the new window. If no rectangle is selected the whole stack is copied.
Ctrl+Shift: Copy only the current slice of the current selection to the new window
Ctrl+Alt: Do not copy any data. Open a new view of the data in the new window

In the graph window the selection is determined by the vertical bars you can drag in from the border (they turn red when they are in use), NOT the rectangle selection. For 4d stacks the following additional rule applies

In add-up and maximum intensity projection mode all layers (along the hidden axis) are copied. In parse-through mode only the current layer is copied.

The Stack Size Dialog
----------------------------

This dialog allows you to change the physical size, offset and pixel dimensions of the stack as well as its data type.

Exporting Data
----------------------------