# Design Patterns Lab - Weather, Editor, and Playlist Systems

![Java](https://img.shields.io/badge/Java-17-blue)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.0-green)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)



## Project Overview

This Spring Boot 3 (Java 17) application demonstrates three fundamental design patterns:
1. **Observer Pattern** for a weather monitoring system
2. **Command Pattern** for a text editor with undo functionality
3. **Iterator Pattern** for a music playlist application

## Design Patterns Implemented

### 1. Observer Pattern (Weather Monitoring System)

**Components:**
- `WeatherStation` (Subject) - Maintains observer list and notifies on changes
- Observer interfaces (`Display`, `StatisticsBoard`, `MobileAlert`)
- Dynamic subscription capability

**Key Features:**
- Loose coupling between subject and observers
- Open/Closed Principle - New observers can be added without modifying subject
- Broadcast notifications to multiple displays

### 2. Command Pattern (Text Editor)

**Components:**
- `Command` interface with `execute()` and `undo()` methods
- Concrete commands (`CutCommand`, `CopyCommand`, `PasteCommand`)
- Invoker class (`TextEditor`) to execute commands
- Command history for undo functionality

**Key Features:**
- Encapsulates each operation as an object
- Supports undo/redo functionality
- Easy to extend with new commands

### 3. Iterator Pattern (Music Playlist)

**Components:**
- `SongIterator` interface with traversal methods
- `Playlist` class managing song collection
- Both forward and reverse iteration support

**Key Features:**
- Abstracts iteration logic from client
- Supports multiple traversal algorithms
- Protects playlist's internal structure

## Getting Started

### Prerequisites

- Java 17 JDK
- Maven 3.8+
- Spring Boot 3.0+

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/design-patterns-lab.git
   cd design-patterns-lab
