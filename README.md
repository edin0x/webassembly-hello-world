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
