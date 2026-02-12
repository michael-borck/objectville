# objectville

An interactive Python tutorial designed to teach object-oriented programming concepts through hands-on exercises and practical examples. This educational project uses a subway system simulation to demonstrate key OOP principles including classes, objects, inheritance, and encapsulation.

## Description

Objectville provides a comprehensive learning experience for students and developers looking to master object-oriented programming in Python. The tutorial centers around a subway system model where learners can explore relationships between different classes, understand data flow, and practice implementing OOP design patterns.

The project is structured as an interactive learning environment that combines theoretical concepts with practical coding exercises, making it ideal for computer science courses, bootcamps, and self-directed learning.

## Installation

### Prerequisites

- Python 3.6 or higher
- Basic understanding of Python syntax and fundamentals

### Setup

1. Clone the repository:
```bash
git clone https://github.com/michael-borck/objectville.git
cd objectville
```

2. Ensure Python is installed and accessible:
```bash
python --version
```

3. No additional dependencies are required - the project uses only Python standard library modules.

## Usage

### Getting Started

Run the main subway system simulation:

```bash
python Subway.py
```

### Core Components

The tutorial is built around several key classes that work together:

**Station Class**
```python
# Example of working with Station objects
from Station import Station

station = Station("Central Station", "CS001")
print(station.get_name())
```

**Connection Class**
```python
# Example of creating connections between stations
from Connection import Connection

connection = Connection(station1, station2, distance=5.2)
```

**Subway System**
```python
# Load and interact with the complete subway system
from Subway import Subway
from SubwayLoader import SubwayLoader

loader = SubwayLoader()
subway = loader.load_from_file("ObjectvilleSubway.txt")
```

### Interactive Learning

1. **Explore the Code Structure**: Start by examining each class file to understand the relationships
2. **Modify Parameters**: Change station names, distances, or connections in the data file
3. **Extend Functionality**: Add new methods or properties to existing classes
4. **Run Simulations**: Use the SubwayPrinter class to visualize different aspects of the system

### Example Exercise

Try modifying the subway system by adding a new station:

```python
# Add this to your learning exercises
new_station = Station("University Campus", "UC001")
# Create connections to existing stations
# Update the subway system and observe the changes
```

## Project Structure

```
objectville/
├── Station.py          # Defines individual subway stations
├── Connection.py       # Manages connections between stations
├── Subway.py          # Main subway system class
├── SubwayLoader.py    # Handles loading subway data from files
├── SubwayPrinter.py   # Provides output formatting and display
├── ObjectvilleSubway.txt  # Sample subway system data
├── output.txt         # Generated output from exercises
└── README.md          # Project documentation
```

## Learning Objectives

Through this tutorial, you will learn:

- **Class Design**: How to structure classes with appropriate methods and attributes
- **Object Relationships**: Understanding composition and association between objects
- **Data Encapsulation**: Implementing proper getter/setter methods and data hiding
- **File I/O**: Reading structured data and creating objects from external sources
- **System Architecture**: Designing interconnected components that work together

## Educational Context

This project was developed for educational purposes and is particularly suited for:

- Computer science students learning OOP concepts
- Python developers transitioning from procedural to object-oriented programming
- Instructors teaching object-oriented design principles
- Self-learners working through programming tutorials

## Configuration

The subway system can be customized by modifying the `ObjectvilleSubway.txt` file. The format follows a structured pattern that the SubwayLoader can parse to create the object network.

## Contributing

This is an educational project. If you're an instructor or student with suggestions for improvements:

1. Fork the repository
2. Create a feature branch for your enhancement
3. Test your changes with the existing codebase
4. Submit a pull request with a clear description of the educational value

## License

This project is intended for educational use. Please refer to your institution's guidelines for academic projects and code sharing policies.