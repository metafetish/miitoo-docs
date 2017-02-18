## Kiiroo Protocol

The Kiiroo communications protocol consists of strings send to either
the Pearl or Onyx. These strings are formatted like so:

```
x,\n
```

Where x is an integer from 0-4. When sent to the Onyx, this command
sets the pressure ring position. When sent to the Pearl, this command
sets vibration levels. 

These commands are sent from the Pearl whenever a corresponding touch
sensor is hit. There is no way to send commands from the Oynx.

That is it. That is the whole protocol. The end.

### Stupid Kiiroo Tricks

The simplicity of the protocol means that two toys can interact
locally on POSIX-compliant platforms (linux, OS X, etc) using nothing
but a 'cat' command. If both toys are paired using Bluetooth 2.0, so
that the Pearl is at

```
/dev/tty.PEARL-DevB 
```

and the Onyx is at

```
/dev/tty.ONYX-DevB
```

Then the following command can be run

```
cat /dev/tty.PEARL-DevB > /dev/tty.ONYX-DevB
```

This will cause the output from the Pearl's touch sensors to be read
directly into the Onyx, controlling its pressure rings.
