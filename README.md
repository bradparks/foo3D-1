foo3D
=====

Crossplatform lowlevel 3D rendering API in Haxe

![foo3D](http://developium.net/pics/w00t3.jpg)

Foo3D is a crossplatform low-level rendering API written in Haxe. It's not a 3D engine. It's supposed to be a crossplatform groundlayer for more sophisticated 3D engines written in Haxe.

Foo3D doesnt make any assumptions about your project-setup. All it needs is a 3D-context in order to work. You are free to allocate a context on your own and hand it over to Foo3D's RenderDevice via DI. Alternatively you can use the supplied utility-classes to receive a window/canvas/stage + context to render to.

## Features:
* Haxe3 ready!
* a common interface across different targets.
* available primitives:
  * Vertexbuffers
  * Textures
  * ShaderPrograms
  * Renderbuffers
* low-level management of GPU-resources
* low-level renderstatemanagement
* optional 3D-context creation(canvas3d, stage3d, glut)
* many samples

## Targets:
* js(webgl)
* flash(stage3D)
* cpp (windows-x86 & ogl)

## Notes:
* Make sure you got foo3d.ndll in your path/sample-folders. It's compiled via hxcpp. Check the content of the "native-bindings"-folder.
* Foo3D uses GLUT for the optional creation of the window and the context. Make sure you got glut32.dll in your path if you use the Frame-Class(like most of the samples).
* On older systems Webgl can be blacklisted in your browser. Try setting "webgl.force-enabled;true" via "about:config".

## Samples:

### 06-Openfl - Openfl SimpleOpenglView + foo3D
![http://developium.net/projects/foo3d/06-Openfl/s_200.jpg]
* See the sample live: [html5](http://developium.net/projects/foo3d/05-Glow/js)