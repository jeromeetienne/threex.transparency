threex.transparency
===================

It is a three.js extension to easily handle transparency.
Here is a [basic example](http://jeromeetienne.github.io/threex.transparency/examples/basic.html).

Show Don't Tell
===============
* [examples/basic.html](http://jeromeetienne.github.io/threex.transparency/examples/basic.html)
\[[view source](https://github.com/jeromeetienne/threex.transparency/blob/master/examples/basic.html)\] :
It shows a basic usage of this extension.

A Screenshot
============
[![screenshot](https://raw.githubusercontent.com/jeromeetienne/threex.transparency/master/examples/images/screenshot-threex-transparency-512x512.jpg)](http://jeromeetienne.github.io/threex.transparency/examples/basic.html)

## How To install it

You can install it manually or with
[bower](http://bower.io/).
for the manual version, first include ```threex.transparency.js``` with the usual

```html
<script src='threex.transparency.js'></script>
```

or with
[bower](http://bower.io/) 
you type the following to install the package.

```bash
bower install -s threex.transparency=https://github.com/jeromeetienne/threex.transparency/archive/master.zip
```

then you add that in your html

```html
<script src="bower_components/threex.transparency/threex.transparency.js"></script>
```

## How To Use It ?

The algo is well described in this
[opengl tutorial about transparency](http://www.opengl-tutorial.org/intermediate-tutorials/tutorial-10-transparency/). We just adapt it to fit three.js.
First you setup all the objects that you want to be transparent

```
THREEx.Transparency.init(objects)
```

It will change the ```THREE.Material``` to make it support transparent.
Second you need to update all your objects at every frame.

```
THREEx.Transparency.update(objects, camera)
```
