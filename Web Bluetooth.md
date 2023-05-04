# Web Bluetooth

![w](https://user-images.githubusercontent.com/116082827/236095872-13f03ff6-5d76-4a15-a0f9-86952350a985.jpeg)


Web Bluetooth allows web applications to communicate with Bluetooth devices, such as sensors and other peripherals. This can be useful for creating web-based IoT applications. The navigator.bluetooth API is used to discover and connect to Bluetooth devices.

Here's an example of how to use Web Bluetooth:





navigator.bluetooth.requestDevice({filters: [{services: ['battery_service']}]})

  .then(device => device.gatt.connect())

  .then(server => server.getPrimaryService('battery_service'))

  .then(service => service.getCharacteristic('battery_level'))

  .then(characteristic => characteristic.readValue())

  .then(value => console.log('Battery Level:', value.getUint8(0)))

  .catch(error => console.error(error));
