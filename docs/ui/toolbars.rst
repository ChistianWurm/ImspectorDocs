========
Toolbars
========

Display toolbar
---------------

The 'Display' toolbar (:ref:`fig_toolbar_display`) allows to change the way the data is displayed in a very fast way.

- The first three buttons allow to rotate a 3D data stack from XY to XZ to YZ.
- The fourth button allows to exchange the displayed X and Y axis and thereby to tilt the data axes.
- The fifth button changes the data representation from overlaid to side by side.
- The sixth button is to show the different data channels in RGB colors. The first channel will be shown in red, the second in green, and the third in blue. All other channels will not be changed.
- The seventh button shows/hides the information and comment pane on top of the measurement view.
- The eighth button shows information on the data stack dimensions.

.. _fig_toolbar_display:
.. figure:: /images/ui/toolbar_display.png
   :width: 8 cm
   :align: center

   The 'Display' toolbar.

Files toolbar
-------------

- The first button of the 'File' toolbar (:ref:`fig_toolbar_files`) creates a **new measurement** with default imaging parameters (which are given during the installation of the microscope).
- The second button of the file toolbar creates a **new measurement from a template** (containing the imaging parameters).
- The third button of the file toolbar **opens** a measurement from a file. Here as well files from other compatible imaging formats can be opened.
- The fourth button of the file toolbar **saves** a measurement with a given file name (**save as**).
- The fifth button of the file toolbar saves a measurement under the same file name the current measurement is entitled with.
- If the 'overwrite warning' is activated Imspector will ask if the current measurement should be overwritten. Otherwise it saves it with the same file name.
  **An already existing file may be overwritten!**
- The sixth button of the file toolbar creates a **new window** within the current measurement.
- The seventh button of the file toolbar **cuts** out the selected data window. The data is purged to the clipboard.
- The eighth button of the file toolbar **copies** the selected data to the clipboard.
- The ninth button of the file toolbar **pastes** the selected data window to the measurement or graph window.

.. _fig_toolbar_files:
.. figure:: /images/ui/toolbar_files.png
   :width: 9 cm
   :align: center

   The 'Files' toolbar.

Measurement toolbar
-------------------

- The first button of the 'Measurement' toolbar (:ref:`fig_toolbar_measurement`) is the 'REC' button. It starts a measurement with the given parameters.
- The second button of the 'Measurement' toolbar pauses a measurement at the point when it is pressed.
- The third button of the 'Measurement' toolbar clones a measurement including the imaging parameters.
- The fourth button of the 'Measurement' toolbar is labeled 'Auto repetition'. When pressed, the measurement is continued until being stopped.

.. note::
   If the 'overwrite warning' is activated Imspector will ask if the current measurement should be overwritten.
   **An already existing file may be overwritten!**

.. _fig_toolbar_measurement:
.. figure:: /images/ui/toolbar_measurement.png
   :width: 4.5 cm
   :align: center

   The 'Measurement' toolbar.

Zoom toolbar
------------

- The first three buttons of the 'Zoom' toolbar (:ref:`fig_toolbar_zoom`) are similar to the ones known from Windows applications: **zoom to selection, zoom in, zoom out**.
- The fourth button of the 'Zoom' toolbar ('Reset Zoom') zooms the data to a scale where one pixel on the screen equals one pixel in the measurement.
- The fifth button of the 'Zoom' toolbar enlarges the measurement window to the size of the shown data (containing the zoom factor).
- The sixth button of the 'Zoom' toolbar shrinks the measurement window to the size of the shown data (containing the zoom factor).
- The seventh button of the 'Zoom' toolbar locks the dimensions of shown data.

.. _fig_toolbar_zoom:
.. figure:: /images/ui/toolbar_zoom.png
   :width: 7 cm
   :align: center

   The 'Zoom' toolbar.
   

PowerSwitch and Microscope Status Toolbar
---------------

- The first button of the 'PowerSwitch and Microscope Status' toolbar (see Fig.) is the 'PowerSwitch' button. In microscopes where   'PowerSwitch' hardware is installed, it is used to switch the microscope hardware on and off. In microscopes where no 'PowerSwitch' hardware is installed, it is used to shut down the STED laser(s). 
- The second button of the toolbar is the Microscope Status button. It displays the microscope status using different symbols:     everything is operating correctly/measurements can be done without limitations (see Fig.); some device shows a notification/measurements can be typically performed – please check status of devices (see Fig.); error status/measurements can not be performed – please check status of devices (see Fig.). Upon pressing the button, the 'Device Status' window will open, indicating the status of the individual devices (see Fig.)

.. _fig_toolbar_PowerSwitch_and_Microscope_Status:
.. figure:: 
   :width: 8 cm
   :align: center

   The 'PowerSwitch and Microscope Status' toolbar.

.. _fig_toolbar_Device_Status:
.. figure:: 
   :width: 8 cm
   :align: center

   The 'Device Status' window. Left, everything runs fine; Right, some devices are not initialized or show errors.
