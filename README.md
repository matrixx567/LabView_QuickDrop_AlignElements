# LabVIEW QuickDrop AlignElements

[![Image](https://www.vipm.io/package/mnprojects_lib_quickdrop_alignelements/badge.svg?metric=installs)](https://www.vipm.io/package/mnprojects_lib_quickdrop_alignelements/) [![Image](https://www.vipm.io/package/mnprojects_lib_quickdrop_alignelements/badge.svg?metric=stars)](https://www.vipm.io/package/mnprojects_lib_quickdrop_alignelements/)

A LabVIEW Quick-Drop (QD) plug-in for aligning and distributing elements on afrontpanel or blockdiagram.

This plug-in is based on the existing [Align & Compress BD/FP Objects](https://forums.ni.com/t5/Quick-Drop-Enthusiasts/Quick-Drop-Plugin-Align-Compress-BD-FP-Objects/gpm-p/3501021?profile.language=en) plug-in. The plug-in is completely refactored and changes the handling and the keymap of the original plug-in.

*Thanks to Jim for his incredible plug-in.*

![Screenshot](../master/docs/screenshot.png)

The design idea behind the usage of the plug-in is to simply handle the alignment using the left hand on the keyboard and the WSAD keys. Therefore you will be very fast to organize your elements on the VI.

**Links / Tutorials**  
https://kreiseder.org/2025/07/quickdrop-alignelements-labview

## Installation

The plug-in is published as a [VIPM Community package](https://www.vipm.io/package/mnprojects_lib_quickdrop_alignelements/). Search for `QuickDrop AlignElements` in the VI Package Manager and install it easily. Otherwise you can download the VIP package from the Release page and install it manually.

## Usage

At first you have to *select some elements*  either on the frontpanel or the blockdiagram of the VI.

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
* `F`: Vertical Compress
* `G`: Horizontal Compress

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

## Numeric controls on the frontpanel

Like the original plug-in the increment and decrement buttons of a numeric control will be hidden during alignment (based on [this idea exchange](https://forums.ni.com/t5/LabVIEW-Idea-Exchange/Align-objects-should-not-align-increment-decrement-buttons/idi-p/1050356?profile.language=en)).

By default this behavior is activated. It is possible to deactivate it in the LabVIEW.ini.

## Position of the Window

Usually the positon of the Quick Drop window will be placed next to the current mouse position. On a MAC computer this won't be able because the `Input Device Control palette` isn't available. For that the Quick Drop window will be placed with an offset to the current FP/BD window. This offset can be
configured using the `LabVIEW.ini`. 

## Quick Drop Options

You can control certain aspects of operation of this plug-in by setting the following LabVIEW.ini tokens:

| Token                                | Default Value      | Description                                                |
| ------------------------------------ | ------------------ | ---------------------------------------------------------- |
| QDAlignElements.HideIncDec           | True               | Hide Inc/Dec buttons of Numeric Controls during alignment. | 
| QDAlignElements.MacWinPosOffsetX     | 200                | Horizontal Offset of QuickDrop Window on MAC.              | 
| QDAlignElements.MacWinPosOffsetY     | 200                | Vertical Offset of QuickDrop Window on MAC.                | 


## Hints

The plug-in is developed with LabVIEW 2020.

