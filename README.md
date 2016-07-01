Dialogger
=========

[![Dialogger](http://i.imgur.com/KliEDM7.png)](http://i.imgur.com/KliEDM7.png)

Dialogger is a simple dialogue graph editor. It saves your dialogue graph in
two file formats:

- **.dl** - JSON file including all visual layout information
- **.json** - (when using "Export..." dialog) Optimized JSON, easier to parse in
    other systems.

It uses [Electron](http://electron.atom.io/) and [JointJS](http://www.jointjs.com/).

Read more about the rationale
[here](http://etodd.io/2014/05/16/the-poor-mans-dialogue-tree/).

Running
-------

Navigate to the project folder install the dependencies with NodeJS + NPM using:

```
npm install
```

After all the dependencies are installed (Electron is an included dependency),
just run it:

```
npm start
```

Usage
-----

Click and drag the grid to navigate around.

Right click on the grid to select the type of node to create:

- **Text** - Create a simple node for a string of text.
- **Choice** - Branch from a text node with multiple options.
- **Branch** - A switch/case list for previously set variables. Click the `+`
    to add more cases and the `-` to remove (from the bottom).
- **Set** - Name and set a variable.
- **Node** - ??? This is identical to Text, so I'm not sure why it's here.

After creating a node, click and drag from the green semicircle of the node to
another node's red semicircle to connect them. You can change which node an
arrow is attached to by clicking and dragging the appropriate end of the
arrow.

Click the X anywhere you see it to delete the attached thing.

The MIT License
---------------

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
