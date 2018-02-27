# qr2mqtt

## Installing

You do not need to install anything. Just visit the following link and use it:

...

*Note:* Chrome requires HTTPS when using the WebRTC API. Any pages using this library should be served over HTTPS.


This project implements a HTML5 based QR code reader which sends all seen codes via MQTT to the specified topic. Therefore it enables you to use your smartphone, tablet or laptop with webcam to be used as cheap QR Scanner in the IoT environment.  

## Credits

It is entirely written in Javascript and utilizes the following components:

* GUI: [Bootstrap](https://getbootstrap.com/) and [jQuery](https://jquery.com/)
* QR Code scan engine: [instascan](https://github.com/schmich/instascan)
* MQTT Client library: [eclipse-paho](https://www.eclipse.org/paho/clients/js/)


## License

Copyright, 2018 bytebang e.U. []
MIT License. See LICENSE for details.
