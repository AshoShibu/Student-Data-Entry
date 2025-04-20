# Student Data Entry System (Java)

## Overview
This Java console-based application provides a simple student data entry system. It supports operations to **add**, **delete**, **search**, and **display** student records using a `Student` class and custom exception handling for better error management and program stability.

---

## Features

- Add new student records
- Delete existing student records
- Search student records by ID
- Display all stored student records
- Use of **custom exceptions** for:
  - Duplicate student ID
  - Student not found
  - Empty student list


---

## How to Run

### Prerequisites
- Java JDK installed
- IDE like IntelliJ/Eclipse OR Terminal

### Steps to Execute
1. Open terminal or IDE and navigate to project folder.
2. Compile all `.java` files:
   ```bash
   javac *.java
   ```
3. Run the program:
   ```bash
   java Main
   ```

---

## Custom Exceptions Used

| Exception Class               | Purpose                                                   |
|------------------------------|-----------------------------------------------------------|
| `DuplicateStudentException`  | Thrown when adding a student with an already existing ID  |
| `StudentNotFoundException`   | Thrown when searching/deleting a non-existing student     |
| `NoStudentsException`        | Thrown when attempting to display an empty student list   |

---

## Functionalities

### `addStudent(Student student)`
- Adds a new student if the ID is unique.
- Throws `DuplicateStudentException` if a student with the same ID already exists.

### `deleteStudent(int id)`
- Deletes the student matching the given ID.
- Throws `StudentNotFoundException` if no student matches the ID.

### `searchStudent(int id)`
- Searches and returns student details by ID.
- Throws `StudentNotFoundException` if not found.

### `getAllStudents()`
- Returns a list of all students.
- Throws `NoStudentsException` if no students are stored.

---

