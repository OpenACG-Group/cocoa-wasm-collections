# Cocoa Prebuilt WebAssembly Collections

<div align="center">
<img width="30%" src="./assets/webassembly-logo.svg">
</div>

Prebuilt WebAssembly modules (including JavaScript loaders) of popular libraries
for [Cocoa](https://github.com/OpenACG-Group/Cocoa).

## Introduction
As Cocoa can be seen as a JavaScript engine based on Google V8, it has full support
of WebAssembly, with JIT compilation for better performance. Cocoa also supports
loading a native library as a language binding, whose APIs can be exported as a
V8 synthetic module and be used in JavaScript. However, writing a language binding
can be hard especially for those large and complicated libraries (e.g. OpenCV),
and it requires you have good knowledge of C++ and Cocoa's internal details.
In that case, if you do not care about the tiny performance loss, WASM is an ideal
choice, as many libraries can be compiled into WASM easily now.

The TypeScript `.d.ts` files and the glue code JS files of officially supported
WASM modules is in `//tslib/wasm` directory of Cocoa project. Tutorials of how
to compile and use them is also in the same directory.

This repository just provides you with the prebuilt WASM modules, which can be
directly used without compiling them by yourself.

## Building Tutorials
Instructions of how to build WASM libraries and make them usable for Cocoa can
be found in `//tslib/wasm` directory of Cocoa project. The final building artifacts
are stored in this repository.
