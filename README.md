# FizzBuzzObjectOrientedEdition

Enterprise software marks a special high-grade class of software that makes careful use of relevant software architecture design principles to build particularly customizable and extensible solutions to real problems.

This is the FizzBuzzObjectOrientedEdition - a satirical implementation of the classic FizzBuzz programming problem using enterprise software design patterns. The project demonstrates over-engineered Java architecture with extensive use of factories, strategies, adapters, and dependency injection.

This is a fork of the original [FizzBuzzEnterpriseEdition](https://github.com/EnterpriseQualityCoding/FizzBuzzEnterpriseEdition) repository.

## About FizzBuzz

FizzBuzz is a game that has gained in popularity as a programming assignment to weed out non-programmers during job interviews. The object of the assignment is less about solving it correctly according to the below rules and more about showing the programmer understands basic, necessary tools such as `if`-/`else`-statements and loops. The rules of FizzBuzz are as follows:

For numbers 1 through 100,

* if the number is divisible by 3 print Fizz;
* if the number is divisible by 5 print Buzz;
* if the number is divisible by 3 and 5 (15) print FizzBuzz;
* else, print the number.

## Getting Started

Welcome to the most object-oriented implementation of FizzBuzz ever created! This guide will help you get this sophisticated business solution up and running on your development environment.

### Prerequisites

Before you can experience the full power of enterprise-grade FizzBuzz, ensure you have the following installed:

#### Required Software

1. **Java Development Kit (JDK) 8 or higher**
   - This project is configured for Java 1.8+ compatibility
   - Tested with OpenJDK 20
   - Download from [Eclipse Temurin](https://adoptium.net/) or [Oracle](https://www.oracle.com/java/technologies/downloads/)

2. **Maven 3.6+ OR Gradle 8.5+**
   - **Maven**: Download from [maven.apache.org](https://maven.apache.org/download.cgi)
   - **Gradle**: Uses included wrapper, no separate installation needed

#### Installation on macOS (via Homebrew)

```bash
# Install Java (if not already installed)
brew install openjdk

# Install Maven
brew install maven

# Verify installations
java -version
mvn -version
```

#### Installation on Linux (Ubuntu/Debian)

```bash
# Install Java
sudo apt update
sudo apt install openjdk-11-jdk

# Install Maven
sudo apt install maven

# Verify installations
java -version
mvn -version
```

#### Installation on Windows

1. Download and install Java JDK from Oracle or Eclipse Temurin
2. Download Maven from the official website and add to PATH
3. Verify installations in Command Prompt:
   ```cmd
   java -version
   mvn -version
   ```

### Setup Instructions

#### 1. Clone the Repository

```bash
git clone https://github.com/andrecasal/FizzBuzzObjectOrientedEdition.git
cd FizzBuzzObjectOrientedEdition
```

#### 2. Choose Your Build Tool

This project supports both Maven and Gradle. Choose one:

##### Option A: Using Maven (Recommended)

```bash
# Compile the project
mvn compile

# Run tests
mvn test

# Build the complete package
mvn package

# Run the application
mvn exec:java -Dexec.mainClass="com.seriouscompany.business.java.fizzbuzz.packagenamingpackage.impl.Main"
```

##### Option B: Using Gradle

```bash
# Make the Gradle wrapper executable (Linux/macOS)
chmod +x gradlew

# Build the project
./gradlew build

# Run the application
./gradlew run
```

#### 3. Expected Output

When you run the application successfully, you should see the classic FizzBuzz output:

```
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
...
(continues to 100)
```

## Architecture Overview

This enterprise-grade solution follows sophisticated architectural patterns and demonstrates over-engineered Java architecture with extensive use of factories, strategies, adapters, and dependency injection.

### Key Components

- **Main Entry Point**: `com.seriouscompany.business.java.fizzbuzz.packagenamingpackage.impl.Main`
- **Spring Framework**: Uses XML-based dependency injection configuration located in `resources/assets/configuration/spring/`
- **Package Structure**: All implementation classes are in `impl/` packages, with corresponding interfaces in `interfaces/` packages
- **Pattern Usage**: Heavy use of Factory pattern, Strategy pattern, Visitor pattern, and Adapter pattern

#### Component Organization

- **Factories**: Located in `impl/factories/` - create instances of strategies, printers, and other components
- **Strategies**: Located in `impl/strategies/` - implement business logic for Fizz, Buzz, and number printing
- **Loop Components**: Located in `impl/loop/` - handle the iteration logic
- **Printers**: Located in `impl/printers/` - handle output formatting
- **String Returners**: Located in `impl/stringreturners/` - return formatted strings

### Dependencies

- Spring Framework 3.2.13 (AOP, Beans, Context, Core, Expression)
- JUnit 4.8.2 for testing
- JaCoCo for code coverage (Maven build)
- javax.annotation-api 1.3.2

### Testing

- Tests are located in `src/test/java/`
- Main test class: `FizzBuzzTest.java`
- Test constants: `TestConstants.java`

## Development Commands Reference

| Task | Maven Command | Gradle Command |
|------|---------------|----------------|
| Compile | `mvn compile` | `./gradlew compileJava` |
| Run Tests | `mvn test` | `./gradlew test` |
| Build Package | `mvn package` | `./gradlew build` |
| Run Application | `mvn exec:java -Dexec.mainClass="..."` | `./gradlew run` |
| Clean Build | `mvn clean` | `./gradlew clean` |

## Troubleshooting

### Common Issues

1. **Java Version Compatibility**
   - Ensure you're using Java 8 or higher
   - The project won't compile with Java 7 or lower

2. **Spring Framework Issues**
   - The project uses Spring 3.2.13 with XML-based configuration
   - Make sure all dependencies are properly downloaded

3. **Build Failures**
   - Try cleaning and rebuilding: `mvn clean compile` or `./gradlew clean build`
   - Check that all dependencies are available in Maven Central

### Still Having Issues?

1. Check the [Issues page](https://github.com/andrecasal/FizzBuzzObjectOrientedEdition/issues) for known problems
2. Verify your Java and Maven/Gradle installations
3. Ensure you have internet connectivity for dependency downloads

## What's Next?

Once you have the application running:

1. Explore the sophisticated architecture in the `src/main/java` directory
2. Examine the Spring configuration files
3. Marvel at the enterprise-grade design patterns
4. Consider the scalability and maintainability of this solution

Remember: This is not just FizzBuzz - this is **OOP FizzBuzz**, designed to showcase object-oriented programming principles taken to their logical extreme!

## Contributing

Although this project is intended as satire, we take openness and inclusivity very seriously. To that end we have adopted the following code of conduct.

[Contributor Code of Conduct](CONTRIBUTING.md)
