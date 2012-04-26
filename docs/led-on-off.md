# Led On Off

```javascript
var five = require("../lib/johnny-five.js"),
    board, led;

board = new five.Board({
  debug: true
});

board.on("ready", function() {

  // Create a standard `led` hardware instance
  led = new five.Led({
    pin: 9
  });

  // "on" turns the led _on_
  led.on();

  // "off" turns the led _off_
  led.off();

  // Turn the led back on after 3 seconds (shown in ms)
  this.wait( 3000, function() {

    led.on();

  });
});

```

## Documentation

_(Nothing yet)_


## Schematics

_(Nothing yet)_



## Contributing
All contributions must adhere to the the [Idiomatic.js Style Guide](https://github.com/rwldrn/idiomatic.js),
by maintaining the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [grunt](https://github.com/cowboy/grunt).

## Release History
_(Nothing yet)_

## License
Copyright (c) 2012 Rick Waldron <waldron.rick@gmail.com>
Licensed under the MIT license.