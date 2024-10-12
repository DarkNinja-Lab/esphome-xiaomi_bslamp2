# Xiaomi Bedside Lamp 2

[ [Changelog](CHANGELOG.md) | [License](LICENSE.md) | [Code of conduct](CODE_OF_CONDUCT.md) ]
 

## Quick start guide

For those who have experience with flashing ESPHome onto devices:

* Make sure you are using ESPHome 2023.4.0 or newer.
* Copy [`example.yaml`](example.yaml) to `<CONFIG_DIR>/<NODE_NAME>.yaml`.
* Modify the configuration to your needs (see the [configuration guide](doc/configuration.md)).
* Compile the `firmware.bin` file and download it to the device to which you have connected your
  serial to USB adapter.
* [Open up the lamp](doc/flashing.md#opening-the-lamp-to-expose-the-pcb) and connect its `TX`, `RX`,
  `GND` and `GPIO0` debug pads to the serial adapter. Check this [image for the debug pad
  locations](doc/images/09_debug_pads_for_soldering.jpg).
* Power up the lamp with `GPIO0` connected to GND to enable flashing mode.
* Flash `firmware.bin` onto the device, for example using
  [esphome-flasher](https://github.com/esphome/esphome-flasher)..
  

