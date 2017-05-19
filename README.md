
A NES emulator in WebAssembly. Based on vNES.

Forked from the C++ version https://launchpad.net/saltynes

# Build
```
./make_web.sh
```

# Run in browser
```
python3 -m http.server 9999
```

TODO
* Move the old SaltyNES to a repo called SaltyNESLegacy
* Update Ui to have copyright
* Make sure all supported mappers actually work
* Auto hide the mouse cursor in fullscteen mode
* Remove resize canvas and pointerlock from ui.
* Make a trivial SDL audio app to see why sound playing is broken.
* Try using opengl for the screen to see if it makes painting faster.
* remove idle messages in web main loop.
* make main loops for desktop and web not have nested while loops
* make fps show in html
* make html terminal show with a toggle button
* make the emulator easy to embed in other web apps by having hooks for all gui buttons
* make it show progress for downloading games and wasm

* Make it not cache the wasm file, even after shift reload
* Is there a way to check if running asm.js instead of WebAssembly?
* Shrink wasm file by removing complex libraries
* Sound is distorted when running in browser, but not desktop
* Change the name
* Make it show a message if WebAssembly is not supported
