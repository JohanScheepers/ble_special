# ble_special

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter BLE application

We will refer to https://github.com/boskokg/flutter_blue_plus as the starting point for the BLE

### Packages

BLE --

    flutter pub add flutter_blue_plus


## BLE

Add permissionds to you android/app/src/main/AndroidManifest.xml

    <manifest xmlns:android="http://schemas.android.com/apk/res/android">
    <!-- Allow Bluetooth -->
     <uses-feature android:name="android.hardware.bluetooth_le" android:required="true" />

    <!-- New Bluetooth permissions in Android 12
     https://developer.android.com/about/versions/12/features/bluetooth-permissions -->
     <uses-permission android:name="android.permission.BLUETOOTH_SCAN" android:usesPermissionFlags="neverForLocation" />
     <uses-permission android:name="android.permission.BLUETOOTH_CONNECT" />

    <application
        android:label="ble_special"
