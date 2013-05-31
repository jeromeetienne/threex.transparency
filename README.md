threex.transparency
===================

extension to easily handle transparency in three.js

## How To Use It ?

First you setup all the objects

```
THREEx.Transparency.init(scene)
```

It will traverse ```THREE.Object3D``` and all its children, to change 
their ```THREE.Material``` appropriatly. It will be done on all the 
objects marked as transparent so ```object.material.transparent === true```.

Second you update all your transparent objects at every frame.

```
THREEx.Transparency.update(scene, camera)
```

## How To Run Examples

to run examples, you may need to install submodules e.g.
[three.js](http://threejs.org/)
or
[require.js](http://requirejs.org/). Just do

```
git submodule init
git submodule update
```

## License

released under MIT license