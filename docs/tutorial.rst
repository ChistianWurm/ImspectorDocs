.. _ShortTutorial:

==============
Short Tutorial
==============

This is a short tutorial that takes you on a tour of some of the more important features of Imspector. If this is the
first time you use the program, it is a good idea to follow it step by step using the test data that should have
been provided to you with the program.


Starting Imspector
****************
Imspector is started by executing the file Imspector.exe, using the shortcut being placed on the desktop of the measurement PC. (The default installation directory is C:\Imspector\.)
During the startup procedure, the software modules will be loaded. 

Imspector Configurations
-----------------
Imspector allows to work with several configurations that may be saved for the individual users and/or usage scenarios. The configurations contain required hardware settings, display options, default measurements settings, etc. 

.. todo:: Empty

The configuration (sub-)folders can be found in the folder C:\Imspector\Config\. 
If a single configuration is located in this folder, it will be automatically loaded. If more configurations e.g. for individual users are placed in that folder, the software will startup with a screen in which you can choose between the different user configurations (see Fig. above). The configuration which was used during the last measurement session will be highlighted. After choosing the desired configuration, Imspector proceeds to the main screen. 
In addition to that, different Imspector versions may be installed at a single measurement PC.


Imspector Measurements
-----------------
Imspector measurements may contain one or multiple windows. Each window is an individual dataset which might contain individual measurement data, instrument parameters, meta data and analyzed data. All windows within a measurement will be saved as a single file within a '.msr' file format. 
The file format can be read by Imspector, Imspector Base, Python and Matlab with the necessary extension (see below). Further it can be exported into several common data formats (see below).
In Imspector the instrument parameters for performing a measurement can be defined through several ways. They can be defined using the easyCommander, through a predefined measurement template, using existing measurements or by defining the settings fully individually on the base of a predefined standard measurement (which is recommended only for experts).


The Smart Way to Start: easyCommander
-----------------
easyCommander is a novel and largely simplified way to define a measurement in Imspector (see Fig.). It is mainly designed to simplify the usage of Imspector in multi-user environments as core facilities. 

.. todo:: Fig.: 'easyCommander' live dialog.

Several standard usage scenarios are implemented in easyCommander. However, to maintain simplicity, advanced functions have to be defined using standard control elements as live dialogs described below.
EasyCommander is intended as an extension to pre-existing usage concepts in Imspector. It is not a novel front end to Imspector, but it is one of several live dialogs. It enables users that are new to the instrument, or are using it only rarely, to operate the microscope.
We expect that new users of the microscope will start using easyCommander and, after being more experienced, will proceed using templates or standard live dialogs to use the complete functionality and flexibility of the microscope. 

.. todo:: Fig.: 'Dye selection' dialog.

In easyCommander many measurement parameters as excitation lasers, detectors... will be chosen automatically. They are predefined and will be loaded upon selecting a dye in the 'Dye selection' dialog (see Fig.). The 'Dye Selection' dialog is an integral part of 'easyCommander'. It can be opened by clicking into the 'Dye' fields on the bottom left of Imspector.

Workflow:
1. Activate easyCommander.
2. Open new measurement.
3. Make settings compatible to easyCommander (To this end, press buttons on the bottom of the 'easyCommander' live dialog.)
4. Select scan mode: XY, XZ, YZ, XYZ, XYT....
5. Select range, pixel size... (see Table)
6. Select scan mode: Confocal, STED, Confocal & STED
7. Select dyes using the 'Dye Selection' dialog (see Fig.)
8. Start the measurement by pressing 'REC'

.. todo:: Table.: Recommended Scan Settings.

Measurement Template
------------
In Imspector a template-driven workflow is implemented. 
Measurement templates are ready-to-use parameter sets that enable a quick start into the use of Imspector and the microscope without the need for the user to be familiar with each and every detail of the microscope and the software. They contain the acquisition parameters (as field of view, pixel size, scan speed, scan direction, dimensionality, activated lasers, activated detectors....) that are required for a type of measurement. As in an Imspector measurement, multiple windows may be included. 
To open a Template select 'File' → 'New' → 'File from Template'...

During installation of the system a set of standard measurements schemes is pre-defined (see Fig.). Based on these templates users can start with several basic measurement. Later, the given templates can be either adapted for the users measurement of interest or new templates can be created by the user. 
In contrast to easyCommander driven work-flows, measurement templates are not restricted to simplified measurement settings, but may contain most parameters that are available in Imspector at a given the setup. 


Loading Data
------------

.. todo:: Empty

Displaying Data
---------------

Magnifying Glass
****************

If you hold down the :kbd:`shift` key and drag with the left mouse button in a window a magnifying glass is
displayed. :kbd:`shift + alt` keys display an even bigger magnifying glass.

When you are pressing the :kbd:`shift` key AFTER starting to drag it will force a vertical or horizontal line when
selecting a line profile.

Shortcuts
*********

* :kbd:`F9 / F10` Fit maximum/minimum.
  In a stack view this adjusts the colormap max/min to the maximum/minimum of the current selection, in a graph view the y-axis scale to the maximum/minimum value between the slider bars.
* :kbd:`Page Up / Down` Go up/down one slice along the third (z-) axis.
  Also pressing the :kbd:`shift` key moves 10, pressing :kbd:`shift + alt` moves 100 slices along the z-axis.
* :kbd:`ctrl + Page Up / Down` Go up/down one layer along the fourth (hidden) axis.
  Also pressing the :kbd:`shift` key moves 10, pressing :kbd:`shift + alt` moves 100 layers along the hidden axis.

Graphs
------

.. todo:: Empty

Drag, Drop, Cut and Paste
----------------------------

Graphs, image stacks and color maps can be dragged and dropped between windows. This is done by pressing the
:kbd:`ctrl` key while dragging with the left mouse button. Color maps can be dragged onto stacks which will then be
displayed using the dropped colormap. For data the following rules apply

* :kbd:`ctrl` Copy all slices of the current selection to the new window. If no rectangle is selected the whole stack
  is copied.
* :kbd:`ctrl + shift` Copy only the current slice of the current selection to the new window
* :kbd:`ctrl + alt` Do not copy any data. Open a new view of the data in the new window

In the graph window the selection is determined by the vertical bars you can drag in from the border (they turn red
when they are in use), NOT the rectangle selection. For 4d stacks the following additional rule applies:

In add-up and maximum intensity projection mode all layers (along the hidden axis) are copied. In parse-through mode only the current layer is copied.

The Change Stack Size Dialog
----------------------------

This dialog allows you to change the physical size, offset and pixel dimensions of the stack as well as its data type.
It can be accessed using the button at the side of the image or via the shortcut :kbd:`ctrl + t`.

.. figure:: /images/ui/change_stack_size_dialog.png
   :width: 10 cm
   :align: center

   Change Stack Size dialog.

Export Data
-----------

Data from Imspector measurements can be exported into several file formats:

- Colormap Tiff files/stacks (.tif/.tiff)
- RGB Tiff files/stacks (.tif)
- binary double files (.dbl)
- Avi files/movies (.avi)
- Visualization toolkit files (.vtk)
- MRC files (.st, .map, .ccp4, .mrc)
- ASCII data files (.dat, .asc)
- Becker&Hickl data files (.sdt)

To export data select the data Stack and select :menuselection:`File --> Export` or use the shortcut :kbd:`ctrl + e` to open the Export Data dialog.
