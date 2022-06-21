# Use

Connect Nodejs program to Alexa

## How to

```js
const Velocity = require("velocity");

let velocity = new Velocity({
  devices: [
    {
      name: "Light One",
      port: 11000,
      handler: function (action) {
        console.log("Light one:", action);
      },
    },
    {
      name: "Light Two",
      port: 11001,
      handler: function (action) {
        console.log("Light Two:", action);
      },
    },
  ],
});
```

### Misc.

You can also connect to `HomeKit` and `Google Home` by setting up `Homebridge` and installing `WeMo` and `Google Home` plugin
