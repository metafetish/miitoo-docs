## Models

Kiiroo currently produces 2 toys, the Pearl and the Onyx.

The Pearl is a dildo with a vibration motor and touch sensors. 

The Onyx is an onahole (silicone hole made for insertion of the penis)
with vibration and pressure motors.

## Bluetooth Information

All Kiiroo toys communicate over both Bluetooth 2.0, using SPP, and
Bluetooth LE, using a single characteristic for sending and other for
receiving.

### Bluetooth 2.0 Connections

When pairing using Bluetooth 2.0, serial ports on OS X and linux
machines will register for the Pearl toy as:

```
/dev/tty.PEARL-DevB 
```

and for the Onyx toy as:

```
/dev/tty.ONYX-DevB
```

### Bluetooth LE Connections

When using Bluetooth LE to talk to Kiiroo toys, the following UUIDs are used.

Service UUID:
```
49535343-fe7d-4ae5-8fa9-9fafd205e455
```

RX Characteristic UUID:
```
49535343-1e4d-4bd9-ba61-23c647249616
```

TX Characteristic UUID:
```
49535343-8841-43f4-a8d4-ecbe34729bb3
```

