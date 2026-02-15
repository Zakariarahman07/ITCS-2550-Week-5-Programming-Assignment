[![C++ doctest](https://github.com/Zakariarahman07/ITCS-2550-Week-5-Programming-Assignment/actions/workflows/c-cpp.yaml/badge.svg)](https://github.com/Zakariarahman07/ITCS-2550-Week-5-Programming-Assignment/actions/workflows/c-cpp.yaml)
# Math Aptitude Analyzer

## Description

The **Math Aptitude Analyzer** is a C++ console application that evaluates a user's math skills, confidence, and study habits, then provides detailed feedback. The program collects personal and academic information, performs calculations, runs a math quiz, and generates formatted report files.  

This project was created for **ITCS 2550 (C++ Programming 2)** and demonstrates **object-oriented programming, file handling, and data validation**.

---

## Features

* Friendly welcome banner with colored console output
* User input collection with validation
* Calculates estimated problems solved per hour
* Stores last five test scores and calculates average
* Five-question math quiz with difficulty levels (Easy, Medium, Hard)
* Instant quiz feedback based on performance and confidence level
* Displays favorite subjects entered by the user
* Demonstrates classes, inheritance, and composition
* Generates formatted output files:

  * `report.txt`

---

## C++ Concepts Demonstrated

* **Selection Statements:** `if / else`, `switch-case`  
* **Loops:** `for`, `while`, `do...while`  
* **Functions:** value-returning and void functions  
* **Arrays:** storing test scores and favorite subjects  
* **Structs:** `LearnerProfile` for storing user info  
* **Enumerations:** quiz difficulty levels (`EASY`, `MEDIUM`, `HARD`) and happiness level (`SAD`, `NEUTRAL`, `HAPPY`)  
* **Classes & Objects:**  
  - Base class: `Person` (name, age, happiness)  
  - Derived classes: `Student` (ID, grade, test score) and `Teacher` (teaching subject, hire date)  
  - Composition class: `Date` (inside `Teacher`)  
* **Inheritance:** Derived classes override base class functionality  
* **Composition:** `Teacher` contains a `Date` object as a member  
* **File Handling:** Writing user reports to `.txt` files using `ofstream`  
* **Input Validation:** Ensures valid data entry for all inputs  
* **Unit Testing:** Using `doctest` to verify constructors, setters, getters, and functions

### Object-Oriented Programming

* **Classes & Inheritance**
  - Base class: `Person` (name, age, happiness)
  - Derived classes: `Student` (ID, grade, test score) and `Teacher` (teaching subject, hire date)
* **Pure Virtual Functions & Abstract Classes**
  - `Person` is abstract
  - Derived classes implement `getSubject()`
* **Polymorphism**
  - `School` stores `Student*` and `Teacher*` as `Person*`
  - Virtual functions `print()` and `getSubject()` allow dynamic dispatch
* **Composition**
  - `Teacher` contains a `Date` object (`hireDate`) to represent hiring date
* **Dynamic Array & Container Class**
  - `School` manages a dynamic array of `Person*`
  - Can **add and remove** objects dynamically
  - Automatically resizes when capacity is exceeded
* **Memory Management**
  - Uses `new` and `delete` for dynamic allocation
  - Virtual destructor ensures derived objects are deleted correctly
  - Prevents memory leaks during removal of objects

---

## How to Run the Program

1. Open **Visual Studio** or **VS Code**  
2. Ensure a C++ compiler is installed  
3. Compile and run `main.cpp`  
4. Follow the on-screen prompts to enter personal info, test scores, and favorite subjects  
5. Complete the five-question math quiz  
6. Review generated output files:

   * `report.txt` → User performance summary  
---

## Example Interaction

```text
Welcome to the Math Aptitude Analyzer! Sharpen your Math skills and discover your true potential!

Enter your full name: John Doe
Enter your favorite Math Subject: Algebra
Enter the number of Math Problems Solved Per Week: 15
On a scale of 1 to 10, how confident are you in Math: 8
Enter number of hours studying Math per week: 5

Enter your last five Algebra test scores:
Test Score 1: 90
Test Score 2: 85
Test Score 3: 92
Test Score 4: 88
Test Score 5: 95

Your average test score in Algebra is: 90.0

Enter Your Favorite Subjects:
Algebra Geometry Trigonometry

Please Complete the Following Five Questions Math Quiz:
Enter difficulty level for the quiz (E for Easy, M for Medium or H for Hard): E
Enter a math operator (+, -, *, /, %): +
5 + 3 = 8
Correct! Well Done!
```
## Student And Teacher Demonstration
```
----- Inheritance and Composition Demonstration -----

Student:
Name: Zakaria Rahman
Age: 20
Happiness Level: Happy
Student ID: 123456
Student Grade: A
Student Test Score: 94
Feedback: Excellent work! Keep up the high performance.

Teacher:
Name: John Koss
Age: 45
Happiness Level: Neutral
Teaching Subject: Computer_Science
Hire Date: 05/20/2003
```
## Output Files

### report.txt

* User name
* Favorite math subject
* Confidence level
* Study hours
* Estimated problems solved per hour
* Test scores and average

---
**Author:** Zakaria Rahman
**Course:** ITCS 2550 – C++ Programming 2







