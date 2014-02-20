*This repository is a mirror of the [component](http://component.io) module [juliangruber/key-pressed](http://github.com/juliangruber/key-pressed). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/juliangruber-key-pressed`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# key-pressed

  Check if one or more keys are currently pressed.

## Usage

```js
var pressed = require('key-pressed')();

// CMD pressed?
pressed([224, 17, 91, 93]);

// Shift pressed?
pressed('shift');

// Shift+CMD pressed?
pressed('shift', [224, 17, 91, 93]);
```

## API

### Pressed([el])

Create an instance listening on `el` or the window object.

### pressed(codes)

Check if `codes` are currently pressed.

All arguments must be pressed, but if an argument is an array, it's enough when one of the codes in that array is pressed.

Supports `keyCode`s, `alt`, `ctrl`, `meta` and `shift.

### pressed.unbind()

Stop listening for events.

## Installation

  Install with [component(1)](http://component.io):

    $ component install juliangruber/key-pressed

## License

  MIT
