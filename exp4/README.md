# Experiment 4: RSS Feed Reader

## Overview

A Flutter application that fetches and displays RSS feed data from a remote server.

## Purpose

This project demonstrates:

- HTTP requests with the http package
- Async/await operations
- Network error handling
- SSL certificate handling
- Data fetching from remote sources
- Scrollable content display

## Features

- ✓ Fetch RSS feed from remote URL
- ✓ Display raw feed content
- ✓ Error handling for network issues
- ✓ Loading state indication
- ✓ Scrollable content area
- ✓ HTTP timeout protection

## RSS Feed Source

Fetches news data from: `http://rss.cnn.com/rss/edition.rss`

## Getting Started

### Installation

```bash
cd exp4
flutter pub get
```

### Running

```bash
flutter run
```

## Project Structure

```
exp4/
├── lib/
│   └── main.dart          # RSS feed fetcher and display
├── pubspec.yaml
└── README.md
```

## Dependencies

- `http: ^1.6.0` - For making HTTP requests

## What You'll Learn

- HTTP client implementation
- Async/await patterns
- Exception handling (ClientException, SocketException)
- Loading states in UI
- Scrollable widgets
- Network request lifecycle

## Technologies Used

- Flutter 3.x
- Dart 3.x
- HTTP package

## Notes

- Requires internet connection
- Uses HTTP URL to avoid SSL certificate issues
