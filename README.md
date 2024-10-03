# Java IntelliJ IDEA and Maven Project

This project demonstrates a simple Java Command Line Interface (CLI) application built with **Maven** and using **Picocli** for command-line parsing. It includes subcommands (`hello` and `goodbye`) to print greetings and farewells, depending on user input. The project also leverages **Maven Shade Plugin** to package the application into a runnable JAR file.

## Table of Contents

- [Prerequisites](#prerequisites)
- [How to Build](#how-to-build)
- [How to Run](#how-to-run)
- [Usage](#usage)

## Prerequisites

To work with this project, you need to have the following installed:

- [Java Development Kit (JDK) 17 or later](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
- [Maven](https://maven.apache.org/install.html)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/download/) (optional, but recommended for development)


## How to Build

To build the project and create the executable JAR file, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd java-intellij-idea-and-maven

2. Use Maven to compile and package the project:
   mvn clean package

   This command will generate the java-intellij-idea-and-maven-1.0-SNAPSHOT.jar file in the target directory.

## How to run 

After building the project, you can run the JAR file using the following command:

java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar "DAI student" hello --greetings "Bonjour"

## Usage

The application has two subcommands: `hello` and `goodbye`. You can use the following options:

1. **hello**: Prints a greeting message.
   - `--greetings`: Specify the greeting message (default: "Hello").

2. **goodbye**: Prints a farewell message.
   - `--farewells`: Specify the farewell message (default: "Goodbye").

### Example Commands

- Run the `hello` subcommand:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar "DAI student" hello --greetings "Bonjour"

  output : Bonjour DAI student!

- Run the `goodbye` subcommand:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar "DAI student" goodbye --farewells "Au revoir"

  output : Au revoir DAI student!

