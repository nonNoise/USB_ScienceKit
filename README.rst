==================================================
USBで始めるお手軽モジュール
==================================================

技術書典４にてご購入ありがとうございます。
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- USBで始める室内環境計測モジュール

	https://github.com/nonNoise/USB_ScienceKit/tree/master/AN-USB-BME280

- USBで始める OLED表示モジュール

	https://github.com/nonNoise/USB_ScienceKit/tree/master/AN-USB-OLED-MINI

- USBで始めるリレー制御モジュール

	https://github.com/nonNoise/USB_ScienceKit/tree/master/AN-USB-Relay

- USBで始めるカラーセンサーモジュール

	https://github.com/nonNoise/USB_ScienceKit/tree/master/AN-USB-S11059

- USBで始めるI2C EEPROMライタ―　モジュール

	https://github.com/nonNoise/USB_ScienceKit/tree/master/AN-USB-EEPROM

Pythonのセットアップについて
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
USBで始めるシリーズは、現在Python"3"をサポートしています。

Python2に関しましては、随時更新を行う予定ですが、出来れば最新のPython3を御利用下さい。

https://www.anaconda.com/download/

よりインストールが可能です。





Q and A
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Q.SCL is low.と表示されて動作しません。

A.I2C通信中にPythonが止まった際に発生します。USBケーブルを一度抜くか、以下の用なソースを起動時に行うと安定します。

	device = PyMCP2221A.PyMCP2221A()

	device.Reset()

	device = PyMCP2221A.PyMCP2221A()