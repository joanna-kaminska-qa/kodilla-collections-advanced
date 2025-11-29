# kodilla-collections-advanced

![Java](https://img.shields.io/badge/Java-21-blue)
![Gradle](https://img.shields.io/badge/Gradle-8-green)
![JUnit](https://img.shields.io/badge/JUnit-5.9.3-purple)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status: Completed](https://img.shields.io/badge/Status-Completed-brightgreen)

This project contains exercises and homework tasks created as part of a module in the **Kodilla "Automated Tester" Java course**, focusing on **Maps and Immutable Maps** in Java 21.  

The module focuses on:
- advanced collections
- immutability
- nested structures
- multimaps
- mapping relationships using Java Maps

The project was developed in **IntelliJ IDEA** as part of the learning path for future **QA/Test Automation Engineers**.


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
├── gradlew / gradlew.bat
├── LICENSE
├── README.md
├── .gradle/
├── .idea/
├── build/
│ ├── classes/java/main/com/kodilla/collections/adv/...
│ └── classes/java/test/com/kodilla/collections/adv/...
└── src/
├── main/java/com/kodilla/collections/adv/
│ ├── exercises/dictionary
│ ├── exercises/homework
│ ├── immutable
│ ├── immutable/homework
│ └── maps
│ ├── complex
│ └── homework
└── test/java/com/kodilla/collections/adv/
├── exercises/dictionary
├── exercises/homework
└── maps
├── complex
└── homework
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

### Dictionary Module
Tests verify:
- Adding words grouped by part of speech
- Multimap-like behavior for storing multiple translations
- Dictionary size and content
- Retrieval of translations

**Test Suite:** `DictionaryTestSuite`

---

### Flight Finder Module
Tests verify:
- Finding flights by departure airport
- Finding flights by arrival airport
- Repository correctness and structure
- Filtering logic based on equality

**Test Suite:** `FlightFinderTestSuite`

---

### Immutability Module
Tests verify:
- Immutable behavior of `Book` and `BookRecord`
- Objects cannot be modified after creation
- Defensive copying ensures safety
- Changes produce new instances instead of modifying originals

**Test Suites:** any test classes covering `Book`, `BookRecord`, and `ImmutableExample`

---

### Maps Module
Tests verify:
- Nested map operations and lookups
- Value summarization (`Grades` class)
- Mapping principals to schools (`SchoolDirectory`)
- Correctness of map-related operations and lookups

**Test Suites:** 
- `BasicMapExampleTest`
- `ComplexMapExampleTest`
- `SchoolDirectoryTest`

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

- **0.3** – Expanded test coverage & structural improvements (achieved >60% total test coverage)
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
  
