threex.transparency
===================

extension to easily handle transparency in three.js


## TODO
* remove require.js submodule
* change API to something more like glow
  * ability to add/remove object transparent

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

Examples are in the ```/examples``` directory. 
to run examples, you may need to install submodules e.g.
[three.js](http://threejs.org/)
or
[require.js](http://requirejs.org/). so just do

```
git submodule init
git submodule update
```

then you need to serve the files in a http server

```
make server
```

and you put [http://127.0.0.1:8000/examples](http://127.0.0.1:8000/examples)
in your browser to try those examples.

## License

released under MIT license