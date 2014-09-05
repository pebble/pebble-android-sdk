pebblekit-android
=================

A software development kit that provides methods for interacting with Pebble
Smartwatch applications.

Watch app ⇆ Android app communications
----------------------------------------
Pebble-enabled Android applications may use the PebbleKit helper class to assist
in sending/receiving data between the watch and the phone.
Developers may refer to the PebbleKitExample class for sample code demonstrating
how Android applications can send data to and receive data from Pebble
Smartwatch applications that support AppMessages.

Android Intent API
------------------
It is also possible to send standard, text-based notifications to Pebble without 
writing a custom watch app, by using the Android Intent API. More information can
be found here: http://developer.getpebble.com/android/intents

Dependencies
------------

* Android SDK >= 2.3.3 (http://developer.android.com/sdk/index.html)

Building a PebbleKitExample APK
-------------------------------

You may use `ant` to build and install an apk.

1. Ensure that the Android SDK is correctly configured and both the `tools/` and `platform-tools/` are on your `PATH`.
2. Execute `ant` in the `pebblekit-android/PebbleKitExample/` directory to see a list of available `ant` targets.

