# LabView QuickDrop AlignElements

A LabVIEW Quick-Drop (QD) plug-in for aligning and distributing elements on afrontpanel or blockdiagram.

This plug-in is based on the existing [Align & Compress BD/FP Objects](https://forums.ni.com/t5/Quick-Drop-Enthusiasts/Quick-Drop-Plugin-Align-Compress-BD-FP-Objects/gpm-p/3501021?profile.language=en) plug-in. The plug-in is completely refactored and changes the handling and the keymap of the original plug-in.

*Thanks to Jim for his incredible plug-in.*

![Screenshot](../master/docs/screenshot.png)

The design idea behind the usage of the plug-in is to simply handle the alignment using the left hand on the keyboard and the WSAD keys. Therefore you will be very fast to organize your elements on the VI.

## Installation
Place the content of the zip file in your `<LabVIEW>\resource\dialog\QuickDrop\plugins` folder.

## Usage

At first you have to *select some elements*  either on the fronpanel or the blockdiagram of the VI.

The Quick Drop plug-in uses the default shortcut `A`.

There are three possible ways to act with the plug-in using the mouse or only the keyboard.

### Using the mouse

With the mouse you can simply act with the plugin

Firstly press `CTRL+SPACE` to open the quick drop dialog, then press `CTRL+A` to open the plug-in dialog containing the alignment and distribution buttons. The different buttons can be pressed to move the objects. At the end the dialog can be closed by clicking on the close button in the corner or by pressing the `ESC` key.

![Using the mouse](../master/docs/usage_mouse.gif)

### Using the keyboard

A faster way to handle this Quick Drop plug-in is by using the keyboard.

After selecting some elements press `CTRL+SPACE` and `CTRL+A` to open the dialog window. Afterwards you can use one of the following keys to execute the wanted alignment:

* `W`: Top
* `S`: Bottom
* `A`: Left
* `D`: Right
* `C`: Horizontal Center
* `V`: Vertical Center
* `Q`: Vertical Gap
* `E`: Horizontal Gap

After pressing a key for alignment the panel will immediatelly be closed.

![Using the keyboard](../master/docs/usage_key.gif)

If you move the mouse pointer over one of the buttons you will see the shortcuts for each operation. (Only some of the distribution elements can be controlled by key.)

![Using the keyboard](../master/docs/tooltips.gif)

### Using the Quick Drop combo box

The last option to handle the plugin is based on Darren's [suggestions](https://forums.ni.com/t5/Quick-Drop-Enthusiasts/Quick-Drop-Plugin-Align-selected-elements/gpm-p/3833359/highlight/true#M1008).

After selecting some elements open the Quick Drop dialog by pressing `CTRL+SPACE`. Insert one or more of the above characters into the combo box. Then press `CTRL+A`. The plug-in will immediatelly execute the alignment or distribution of the elements.

![Using the combo box](../master/docs/usage_combo.gif)

On of my favorites is to open the Quick Drop with `CTRL+SPACE`. Then insert `AQ` into the combo box and press `CTRL+A`. This will align the elements to the left and distribute it with an equal vertical gap. I use this to arrange the VI input and output elements on the blockdiagram.  

![Using the combo box](../master/docs/usage_combo2.gif)

## Hints
The plug-in is developed in LabVIEW 2017. The released ZIP file contains VIs that are converted to LabView 2016. If you have an older version of LabView you have to save the provided project to this older version by yourself.
