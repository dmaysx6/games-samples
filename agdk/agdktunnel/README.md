# AGDKTunnel

A sample project demonstrating use of the Android Game Development Kit libraries.
AGDKTunnel is derived from the NDK sample Endless Tunnel.

AGDKTunnel uses the following AGDK libraries:

* Android Performance Tuner
* Frame Pacing
* GameActivity
* GameController
* GameTextInput
* Oboe

## Prerequisites

### Python

Python is expected to be available in your `PATH`. The `protobuf` package is
expected to have been installed via `pip`. It is expected that `python`
is version 3, not version 2.

NOTE: If you are building on Windows, Android Studio may be using its own local
Python install. Using the `Terminal` tab in Android Studio you can check
for protobuf using `pip list`. If the protobuf package is not present it can be
installed by running `pip install protobuf` from the Terminal tab.

### Note for macOS developers

The runtime data files for Android Performance Tuner are compiled using the
`protoc` compiler located in `third_party/protobuf-3.0.0/install/mac/bin/protoc`.
This executable is not codesigned or notarized. You may need to adjust your
Gatekeeper settings or compile your own protoc from the [protobuf](https://github.com/protocolbuffers) repo to build the project if you encounter errors about
an unsigned executable.

## Building

Open the `agdktunnel' directory in Android Studio 4.2 or higher.

## Android Performance Tuner API Key

The APT functionality requires a valid API key to operate. This is not
necessary to run the sample. For information on configure an API key
for APT, see the **Get an API key for the Android Performance Tuner**
section of the Codelab [Integrating Android Performance Tuner into your native Android game](https://developer.android.com/codelabs/android-performance-tuner-native#1).