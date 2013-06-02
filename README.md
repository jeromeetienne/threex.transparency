threex.transparency
===================

extension to easily handle transparency in three.js

## How To Use It ?

First you setup all the objects that you want to be transparent

```
THREEx.Transparency.init(objects)
```

It will change the ```THREE.Material``` to make it support transparent.
Second you need to update all your objects at every frame.

```
THREEx.Transparency.update(objects, camera)
```

## How To Run Examples

Examples are in the ```/examples``` directory. 
to run examples, you may need to install submodules e.g.
[three.js](http://threejs.org/)

```
git submodule update --init
```

then you need to serve the files in a http server. You can do so with 

```
python -m SimpleHTTPServer
```

and you put [http://127.0.0.1:8000/examples](http://127.0.0.1:8000/examples)
in your browser to try those examples.

## License

released under MIT license