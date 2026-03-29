# Experiment 6: SQLite Database

## Overview

A Flutter application demonstrating SQLite database creation and initialization for local data persistence.

## Purpose

This project demonstrates:

- SQLite database setup with sqflite package
- Database initialization and versioning
- Table creation with schema definition
- Database path management
- Local data persistence

## Features

- ✓ Create SQLite database
- ✓ Create 'student' table with id and name columns
- ✓ Database initialization on app startup
- ✓ Persistent local storage
- ✓ Database versioning support

## Getting Started

### Installation

```bash
cd exp6_create_sqlite_db
flutter pub get
```

### Running

```bash
flutter run
```

## Project Structure

```
exp6_create_sqlite_db/
├── lib/
│   └── main.dart          # Database initialization
├── pubspec.yaml
└── README.md
```

## Dependencies

- `sqflite: ^2.4.2` - SQLite database package
- `path: ^1.9.1` - Path provider for database location

## Database Schema

```sql
CREATE TABLE student (
  id INTEGER PRIMARY KEY,
  name TEXT
)
```

## What You'll Learn

- sqflite package usage
- Database initialization patterns
- Table creation with CREATE TABLE
- Database versioning
- onUpgrade callbacks
- getDatabasesPath()

## Future Extensions

- Add INSERT operations
- Add SELECT/READ operations
- Add UPDATE operations
- Add DELETE operations
- Create a UI for CRUD operations

## Technologies Used

- Flutter 3.x
- Dart 3.x
- SQLite
- sqflite package
