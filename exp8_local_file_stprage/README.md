# Experiment 8: Local File Storage

## Overview

A Flutter application demonstrating reading and writing files to the device's local storage using path_provider.

## Purpose

This project demonstrates:

- File I/O operations in Flutter
- Getting application document directory
- Writing data to files
- Reading data from files
- File existence checking
- path_provider package usage

## Features

- ✓ Write text data to local file
- ✓ Read text data from local file
- ✓ Get application documents directory
- ✓ Check file existence
- ✓ Display file content in UI
- ✓ Error handling for missing files

## Getting Started

### Installation

```bash
cd exp8_local_file_stprage
flutter pub get
```

### Running

```bash
flutter run
```

## Project Structure

```
exp8_local_file_stprage/
├── lib/
│   └── main.dart          # File read/write operations
├── pubspec.yaml
└── README.md
```

## Dependencies

- `path_provider: ^2.1.5` - Access application directories

## File Operations

### Write Data

```dart
Future<void> writeData() async {
  final path = await getFilePath();
  File file = File(path);
  await file.writeAsString("Flutter File Storage Example");
}
```

### Read Data

```dart
Future<void> readData() async {
  final path = await getFilePath();
  File file = File(path);
  if (await file.exists()) {
    String text = await file.readAsString();
    setState(() { fileData = text; });
  }
}
```

## What You'll Learn

- File class for file operations
- path_provider for directory access
- writeAsString() method
- readAsString() method
- File.exists() check
- Async file I/O patterns
- Error handling for missing files

## File Location

- **Path:** Application Documents Directory
- **File Name:** data.txt
- **Platform specific:**
  - Android: `/data/data/com.example.app/files`
  - iOS: `Documents/`

## Technologies Used

- Flutter 3.x
- Dart 3.x
- path_provider package
- dart:io File class

## Future Extensions

- Add UI buttons for read/write operations
- Support multiple files
- JSON serialization
- Encryption for sensitive data
