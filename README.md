# A-Frame `no-click-look-controls` Component

##Overview
Intuitive look controls for desktop 3D experiences. Demo: (coming soon) [alexrkass.com/no-click-look-controls](https://alexrkass.com/no-click-look-controls)

##Features
* :no_entry_sign::arrow_left::arrow_right::no_entry_sign:Includes rotation angle options for dynamically focusing the user on parts of a scene.
* :computer: Provides intuitive desktop view controls without requiring mousedown+drag. 
* :100::sunglasses::iphone: Includes the standard touch and HMD view controls for drop-in replacement for standard `look-controls` component.

##Options

Property      | Default | Description
--------------|---------|-------------
maxyaw        | 3π      | Controls the max y-axis rotation. Actual max viewing angle is twice the parameter, ie 3π          is 3π to the right and 3π to the left.
maxpitch      | π/2     | Controls the max x-axis rotation. Actual max viewing angle is twice the parameter, ie π/2 is π/2 up and π/2 down.
enabled       | true    | Enables controls

##Usage
####Script
```html
<html>
  <head>
    <!-- A-Frame Library -->
    <script src="https://aframe.io/releases/latest/aframe.js"></script>

    <!-- Component -->
    <script src="aframe-gamepad-controls.js"></script>
  </head>
  <body>
    <a-scene>
      <!-- ... -->
      <a-entity camera no-click-look-controls></a-entity>
    </a-scene>
  </body>
</html>
```
####NPM

Install NPM module.

```
$ npm install no-click-look-controls
```

Register `aframe-no-click-look-controls` component.

```javascript
var AFRAME = require('aframe-core');
var NoClickLookControls = require('aframe-no-click-look-controls');
AFRAME.registerComponent('no-click-look-controls', NoClickLookControls);
```

Add markup.

```html
<a-entity camera no-click-look-controls></a-entity>
```
