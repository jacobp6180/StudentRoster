# Student Roster

A console-based C++ application that parses and manages student records for a course roster. The program demonstrates object-oriented programming, data parsing, validation, filtering, and dynamic object management.

## Features

- Parses comma-separated student data into `Student` objects
- Stores and manages students through a `Roster` class
- Displays all students in the current roster
- Calculates each student's average number of days across three courses
- Identifies invalid email addresses
- Filters students by degree program
- Removes students by ID and reports invalid removal attempts

## Technologies and Concepts

- C++
- Object-oriented programming
- Classes, constructors, and destructors
- Encapsulation with getters and setters
- Enumerations
- Arrays and pointers
- String parsing and input validation

## Project Structure

```text
StudentRoster/
├── Degree.h      # Degree-program enumeration and display values
├── Student.h     # Student class declaration
├── Student.cpp   # Student class implementation
├── Roster.h      # Roster class declaration
├── Roster.cpp    # Roster parsing and management logic
└── Main.cpp      # Sample data and program workflow
```

## Getting Started

### Prerequisites

- A C++ compiler with C++11 support or newer, such as GCC, Clang, or Microsoft Visual C++

### Build and Run with GCC or Clang

Clone the repository:

```bash
git clone https://github.com/jacobp6180/StudentRoster.git
cd StudentRoster
```

Compile the source files:

```bash
g++ -std=c++11 Main.cpp Roster.cpp Student.cpp -o student-roster
```

Run the program:

```bash
./student-roster
```

On Windows Command Prompt, run `student-roster.exe` after compiling.

## How It Works

The application begins with a set of comma-separated student records. `Roster::parse()` separates each record into individual fields and passes them to `Roster::add()`, which creates a `Student` object and adds it to the class roster.

The program then:

1. Prints the complete roster.
2. Reports malformed email addresses.
3. Calculates the average number of days each student spends in three courses.
4. Displays students enrolled in the software degree program.
5. Removes a student and demonstrates error handling for a repeated removal request.

## Background

This project was created for WGU's C867: Scripting and Programming - Applications course to practice core C++ and object-oriented programming concepts.
