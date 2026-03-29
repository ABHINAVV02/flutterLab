# Experiment 7: GPS Location Tracker

## Overview

A Flutter application that retrieves the device's GPS coordinates using the geolocator package and permission handling.

## Purpose

This project demonstrates:

- Device location permission handling
- GPS/Geolocation services
- Location accuracy settings
- Permission request flow
- Location service status checking
- Error handling for location failures

## Features

- ✓ Get current device location
- ✓ Request location permissions
- ✓ Check location service status
- ✓ Handle permission denials
- ✓ Display latitude and longitude
- ✓ High-accuracy location tracking

## Getting Started

### Installation

```bash
cd exp7_gps_location_app
flutter pub get
```

### Running

```bash
flutter run
```

## Permissions Required

### Android (AndroidManifest.xml)

```xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
```

### iOS (Info.plist)

```xml
<key>NSLocationWhenInUseUsageDescription</key>
<string>This app needs your location</string>
```

## Project Structure

```
exp7_gps_location_app/
├── lib/
│   └── main.dart          # Location tracking
├── android/
├── ios/
├── pubspec.yaml
└── README.md
```

## Dependencies

- `geolocator: ^14.0.2` - Location services

## What You'll Learn

- Permission handling flow
- Geolocator package usage
- LocationSettings configuration
- LocationAccuracy levels
- Service status checking
- Permission states handling

## Permission States

- `denied` - Permission not yet requested
- `deniedForever` - User permanently denied
- `granted` - Permission granted
- `restricted` - Restricted by system
- `unableToDetermine` - Cannot determine

## Technologies Used

- Flutter 3.x
- Dart 3.x
- geolocator package

## Notes

- Requires physical device or emulator with location services
- Enable location services on device
- Grant permissions when prompted
