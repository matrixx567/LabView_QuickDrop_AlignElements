# LabView QuickDrop AlignElements

A LabVIEW Quick-Drop (QD) plug-in for aligning a selection of elements.

This plug-in is based on the existing [Align & Compress BD/FP Objects](https://forums.ni.com/docs/DOC-14469) plug-in. The plug-in was completely refactored and changes the handling and the keymap of the original plug-in.

![Screenshot](../master/screenshot.png)

## Installation
Place the content of the zip file in your `<LabVIEW>\resource\dialog\QuickDrop\plugins` folder.

## Usage

Select some elements on the frontpanel or the blockdiagram.
Press `Ctrl+Space` `Ctrl+S` to open a small UI with alignment buttons next to the current mouse pointer position.

If a button is pressed the selection of elements will be aligned or distributed to the wanted choice.
The panel can be closed using the window's close button or by pressing the ESC key.

It is also possible to align the elements with the WASD-keys
* `W`: Top
* `S`: Bottom
* `A`: Left
* `D`: Right
* `C`: Horizontal Center
* `V`: Vertical Center
If the alignment is controlled by the keys the panel will immediately be closed.

## Hints
The plug-in is developed with LabVIEW 2016.

The default shortcut for this plug-in is based on the key `S` because on key `A` I usually use the [Align front panel controls to connector pane pattern](https://forums.ni.com/docs/DOC-136239) plug-in.

## License

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

