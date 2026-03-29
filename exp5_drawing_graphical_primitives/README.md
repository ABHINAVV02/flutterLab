# Experiment 5: Graphics and Drawing

## Overview

A Flutter application demonstrating how to draw graphical primitives (shapes) on a canvas using CustomPaint.

## Purpose

This project showcases:

- CustomPaint widget for custom graphics
- Canvas drawing operations
- Paint styling properties
- Geometric shape rendering
- Custom painter implementation

## Features

- ✓ Draw circles using canvas.drawCircle()
- ✓ Draw rectangles using canvas.drawRect()
- ✓ Fill colors on shapes
- ✓ Offset and size control
- ✓ Custom paint styling

## Getting Started

### Installation

```bash
cd exp5_drawing_graphical_primitives
flutter pub get
```

### Running

```bash
flutter run
```

## Project Structure

```
exp5_drawing_graphical_primitives/
├── lib/
│   └── main.dart          # Canvas drawing and ShapePainter
├── pubspec.yaml
└── README.md
```

## What You'll Learn

- CustomPainter class implementation
- Canvas API
- Paint class and styling
- Offset and Rect constructors
- shouldRepaint lifecycle
- Coordinate system in Flutter

## Shapes Drawn

1. **Circle** - Blue filled circle at offset (150, 150) with radius 50
2. **Rectangle** - Blue filled rectangle from (50, 250) with width 200, height 100

## Technologies Used

- Flutter 3.x
- Dart 3.x

## Customization Ideas

- Add more shapes (lines, arcs, paths)
- Add animation
- Add touch interaction
- Change colors dynamically
