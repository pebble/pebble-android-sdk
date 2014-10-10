PebbleKit Android
=================

Welcome to Pebble's official Android SDK!

## Communication with Pebble

On Android, all communication between apps and Pebble go through the official Pebble Android
application via intents.

PebbleKit Android provides a convenience layer on top of those intents.

## Documentation

 - [Using PebbleKit Android](https://developer.getpebble.com/2/mobile-app-guide/android-guide.html/) describes
 how to use PebbleKit Android in your application.
 - [PebbleKit Android API Reference](http://pebble.github.io/pebble-android-sdk)

## Examples

All Pebble examples are now [available on GitHub](https://github.com/pebble/pebble-sdk-examples).

We provide several examples of Android application communicating with Pebble:

 - The [weather demo](https://github.com/pebble/pebble-sdk-examples/tree/master/weather-demo/WeatherDemo-Android) 
 shows how to build an Android application that fetches the weather from the Internet and
 sends it to an app on Pebble ([using the AppSync framework](https://developer.getpebble.com/2/guides/app-phone-communication.html)).
 - The [Sports demo](https://github.com/pebble/pebble-sdk-examples/tree/master/sports-demo/SportsDemo-Android) 
 shows how to build an Android application that starts and communicates with the Sports
 app embedded in all Pebbles.
 - The [Golf demo](https://github.com/pebble/pebble-sdk-examples/tree/master/golf-demo/GolfDemo-Android) shows 
 how to build an Android application that starts and communicates with the Golf app
 embedded in all Pebbles.
 - The [Ocean Survey demo](https://github.com/pebble/pebble-sdk-examples/tree/master/data-logging-demo/OceanSurveyDemo-Android) 
 shows how to build an Android application that leverages data logging to receive
 information pushed by a Pebble app.

## Using PebbleKit Android

As of version 2.5, PebbleKit Android is distributed as a library on the [Sonatype OSS Repository](https://oss.sonatype.org/).
Source code and library (`.aar`) are also available.

You must install the official [Pebble Android application](https://play.google.com/store/apps/details?id=com.getpebble.android)
to use PebbleKit Android.

PebbleKit Android requires Android SDK version 14 or higher (4.0 and above).

### Using PebbleKit Android with Maven

If you are using Maven, you can add the following dependency in your `pom.xml`:

    <dependency>
      <groupId>com.getpebble</groupId>
      <artifactId>pebblekit</artifactId>
      <version>2.5.0</version>
      <type>aar</type>
    </dependency>

### Using PebbleKit Android with Android Studio and Gradle

In Android Studio, or on any Gradle project, you can add PebbleKit Android in your `app/build.gradle` file:

    dependencies {
        compile 'com.getpebble:pebblekit:2.5.0'
    }

Make sure that you also include a reference to the Sonatype OSS Repository:

    repositories {
        mavenCentral()
        maven { url "https://oss.sonatype.org/content/groups/public/" }
    }

### Using PebbleKit Android library directly

Finally you can also [download the AAR file][aar-download] for PebbleKit Android and add it directly into your project.

## Changelog

### 2.5.0 - August 2014

 - (Bumped version to 2.5 to follow firmware updates)
 - Automatic publication to Sonatype OSS Repo

## 2.0 - January 2014

 - First release of 2.0 SDK with the new DataLogging API

[aar-download]: https://oss.sonatype.org/service/local/repositories/releases/content/com/getpebble/pebblekit/2.5.0/pebblekit-2.5.0.aar
