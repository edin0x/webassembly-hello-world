# Innovation day - Webassembly hello world

## Setup
```
$ git clone https://github.com/juj/emsdk.git
$ cd emsdk
$ ./emsdk install sdk-incoming-64bit binaryen-master-64bit
$ ./emsdk activate sdk-incoming-64bit binaryen-master-64bit
$ source ./emsdk_env.sh
```

## Compile and run it
Compile with: `emcc hello.c -s WASM=1 -o hello.html`
Run it: `emrun --no_browser --port 8080 .`

## Reading material
* https://hacks.mozilla.org/2017/02/a-cartoon-intro-to-webassembly/

## Tools
* http://mbebenita.github.io/WasmExplorer/ - WebAssembly Explorer with which you can compile C/C++ code into WebAssembly. Provides also browser specific machine code output.
* https://wasdk.github.io/WasmFiddle/ - Wasm Fiddle. Similar to Wasm Explorer, but besides compiling C/C++, let's you also run the code in the browser.
