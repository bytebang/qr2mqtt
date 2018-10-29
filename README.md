# qr2mqtt

This project implements a HTML5 based QR code reader which sends all seen codes via MQTT to the specified topic. Therefore it enables you to use your smartphone, tablet or laptop with webcam to be used as cheap QR Scanner in the IoT environment.

## Installing

You do not need to install anything. Just visit the following link and use it:

[Try the latest live demo](https://tinyurl.com/qr2mqtt)

*Note:* The application behind this link points to the most recent version of the application.
It will improove / change in the future - so dont expect a stable version here.

If you need a stable version then download the [source file](https://raw.githubusercontent.com/bytebang/qr2mqtt/master/scanner.html) to your device and open it from there. 

## Using

The default parameters are pointing to a public broker with (more ore less) meaningful default values. However, you can set any of the GUI values using URL parameters. For example
`https://rawgit.com/bytebang/qr2mqtt/master/scanner.html?host=something.noip.org&port=8080&tls=false&topic=house/1st_floor/signaling&lastWill=This is the end` will give you the latest version of the scanner which points to the broker `something.noip.org` at the port `8080` without TLS and `house/1st_floor/signaling` as the suggested topic. If the scanner is disconnected, then the last will `This is the end` will be published.

## Compatibility

I have tested the app with chrome on Android and Firefox & Chrome under Linux. It should work with other versions too.
If you have any questions or wishes then please create an [issue](https://github.com/bytebang/qr2mqtt/issues) here in github.


## Credits

It is entirely written in Javascript and utilizes the following components:

* GUI: [Bootstrap](https://getbootstrap.com/) and [jQuery](https://jquery.com/)
* QR Code scan engine: [instascan](https://github.com/schmich/instascan)
* MQTT Client library: [eclipse-paho](https://www.eclipse.org/paho/clients/js/)


## License

Copyright, 2018 [bytebang e.U.](http://www.bytebang.at)
MIT License. See LICENSE for details.
