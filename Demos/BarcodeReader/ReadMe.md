# Barcode reader demo

## Description

This demonstrates the use of the [Google MLVision API to scan barcodes](https://developers.google.com/ml-kit/vision/barcode-scanning/android). It has been tested using Delphi 10.4.2, however it may work on earlier versions.

~~The demo uses a TakePhotoFromCameraAction to capture the image - the code the processes the image to detect barcodes could possibly use images captured "on-the-fly" through video capture.~~

**UPDATE: Due to improvements in TCameraComponent for Android, the demo now uses that for "on-the-fly" detection**

## Android 

The following jar files are used by the project:

* play-services-vision-17.0.2.jar
* play-services-vision-common-17.0.2.jar

Both are located in the [`ThirdParty\Android`](https://github.com/DelphiWorlds/Kastri/tree/master/ThirdParty/Android) folder

If you are creating a new project (i.e. other than the demo) you will need to add these jars to the `Libraries` node under the Android platform in Project Manager

## iOS

On iOS, the demo is dependent on prebuilt libraries in the [`ThirdParty\iOS`](https://github.com/DelphiWorlds/Kastri/tree/master/ThirdParty/iOS) folder

The MLKitBarcodeScanning framework is over 100MB, so it has been zipped (`MLKitBarcodeScanning.framework.zip`). **It will need to be unzipped in place, in order for the app to compile**

If you are creating a new project (i.e. other than the demo) you will need to add the path to the 

* Framework search path, and:
* Search path

..in the project options

![Example](./Screenshots/BarcodeScanExample.png)