# kodilla-collections-advanced

![Java](https://img.shields.io/badge/Java-21-blue)
![Gradle](https://img.shields.io/badge/Gradle-8-green)
![JUnit](https://img.shields.io/badge/JUnit-5.9.3-purple)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

This project contains exercises and homework tasks created as part of a module in the **Kodilla "Automated Tester" Java course**, focusing on Maps in Java 21.  
The module focuses on advanced collections, immutability, nested structures, multimaps, and mapping relationships using Java Maps.

---

## Description

This repository includes Java 21 code demonstrating advanced usage of the **Java Collections Framework**.

### Main topics covered

#### **Advanced Collections**
- complex `Map` structures
- mapping keys to multiple values
- nested collections (`Map<String, List<String>>`, `Map<School, Principal>`)
- dictionary-like behavior (multimap simulation)

#### **Immutability**
- immutable objects
- creating immutable copies
- defensive copying
- using records (`BookRecord`)

#### **Custom Data Structures**
- dictionary module built with:
    - `PartOfSpeech` enum
    - `EnglishWord` class
    - multimap-style word storage

#### **Practical Homework: Flights**
- storing flight data in a repository
- searching by arrival / departure
- filtering logic in `FlightFinder`
- clean API-style search methods

#### **Maps**
- basic maps
- complex maps
- maps with custom objects as keys
- value summarization (`Grades`, `SchoolDirectory`)

All exercises were developed in **IntelliJ IDEA** as part of the Kodilla learning path for QA/Test Automation specialization.

---

## Project Structure

```
kodilla-collections-advanced/
├── build.gradle
├── gradlew
├── gradlew.bat
├── LICENSE
├── README.md
│
├── .gradle/
│   └── 8.13/...
│
├── .idea/
│   ├── compiler.xml
│   ├── gradle.xml
│   ├── misc.xml
│   ├── workspace.xml
│   └── vcs.xml
│
├── build/
│   ├── classes/java/main/com/kodilla/
│   │   ├── Main.class
│   │   └── collections/adv/
│   │       ├── exercises/
│   │       │   ├── dictionary/
│   │       │   │   ├── Dictionary.class
│   │       │   │   ├── EnglishWord.class
│   │       │   │   └── PartOfSpeech.class
│   │       │   └── homework/
│   │       │       ├── Flight.class
│   │       │       ├── FlightFinder.class
│   │       │       └── FlightRepository.class
│   │       ├── immutable/
│   │       │   ├── Book.class
│   │       │   ├── BookRecord.class
│   │       │   ├── ImmutableExample.class
│   │       │   └── homework/
│   │       │       └── Task.class
│   │       └── maps/
│   │           ├── BasicMapExample.class
│   │           ├── complex/
│   │           │   ├── ComplexMapExample.class
│   │           │   ├── Grades.class
│   │           │   └── Student.class
│   │           └── homework/
│   │               ├── Principal.class
│   │               ├── School.class
│   │               └── SchoolDirectory.class
│   │
│   ├── classes/java/test/com/kodilla/collections/adv/
│   │   ├── exercises/dictionary/DictionaryTestSuite.class
│   │   └── exercises/homework/FlightFinderTestSuite.class
│   │
│   └── libs/kodilla-collections-advanced-1.0-SNAPSHOT.jar
│
└── src/
    ├── main/java/com/kodilla/
    │   ├── Main.java
    │   └── collections/adv/
    │       ├── exercises/
    │       │   ├── dictionary/
    │       │   │   ├── Dictionary.java
    │       │   │   ├── EnglishWord.java
    │       │   │   └── PartOfSpeech.java
    │       │   └── homework/
    │       │       ├── Flight.java
    │       │       ├── FlightFinder.java
    │       │       └── FlightRepository.java
    │       ├── immutable/
    │       │   ├── Book.java
    │       │   ├── BookRecord.java
    │       │   ├── ImmutableExample.java
    │       │   └── homework/
    │       │       └── Task.java
    │       └── maps/
    │           ├── BasicMapExample.java
    │           ├── complex/
    │           │   ├── ComplexMapExample.java
    │           │   ├── Grades.java
    │           │   └── Student.java
    │           └── homework/
    │               ├── Principal.java
    │               ├── School.java
    │               └── SchoolDirectory.java
    │
    ├── main/resources/
    └── test/java/com/kodilla/collections/adv/
        ├── exercises/dictionary/DictionaryTestSuite.java
        └── exercises/homework/FlightFinderTestSuite.java
```

---

## Getting Started

### Dependencies

From `build.gradle`:

```gradle
plugins {
    id 'java'
}

group = 'com.kodilla'
version = '1.0-SNAPSHOT'

repositories {
    mavenCentral()
}

dependencies {
    testImplementation 'org.junit.jupiter:junit-jupiter-api:5.9.3'
    testRuntimeOnly 'org.junit.jupiter:junit-jupiter-engine:5.9.3'
}

test {
    useJUnitPlatform()
}
```

---

## Test Suites Overview

### **Dictionary Module**
Tests verifying:

- adding words grouped by part of speech
- multimap-like behavior
- dictionary size and content
- retrieval of translations

### **Flight Finder Module**
Tests verifying:

- finding flights by departure airport
- finding flights by arrival airport
- repository structure and correctness
- equality-based filtering logic

### **Immutability Module**
Tests focus on:

- verifying immutable behavior of `Book` and `BookRecord`
- ensuring objects cannot be modified
- checking defensive copying
- confirming that changes produce new instances

### **Maps Module**
Tests cover:

- nested map operations
- value summarization (`Grades`)
- mapping principals to schools
- verifying correctness of map lookups

These tests help build strong practical understanding of designing and verifying advanced collections and relationships between objects.

---

## Optional Terminal Commands

**Build the project:**

```bash
./gradlew build
```

**Run all tests:**

```bash
./gradlew test
```

**Clean build files:**

```bash
./gradlew clean
```

---

## Authors

Created by:

**Joanna Kamińska**  
GitHub: https://github.com/joanna-kaminska-qa

---

## Version History

- **0.2** – README added, improved documentation
- **0.1** – Initial upload

---

## License

This project is licensed under the **MIT License**.  
See the `LICENSE` file for details.

---

## Acknowledgments

- Kodilla "Automated Tester" Java course
- Java documentation
- JUnit documentation
- Oracle Collections Framework documentation  
