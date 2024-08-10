# NameApp

`NameApp` is a simple Java application that serializes a `User` object into a JSON string and prints it to the console using the `Jackson` library. The project includes a unit test to verify the serialization logic.

## Project Structure
```css
NameApp/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── org/
│   │           └── example/
│   │               ├── NameApp.java
│   │               └── dto/
│   │                   └── User.java
│   ├── test/
│   │   └── java/
│   │       └── org/
│   │           └── example/
│   │               └── NameAppTest.java
└── build.gradle
```

## Dependencies
The project uses the following dependencies:

- **Jackson Databind**: A library for serializing and deserializing Java objects to and from JSON.
- **JUnit 5**: The testing framework used for writing and running the unit tests. 

These dependencies are managed via Gradle and will be automatically downloaded from Maven Central during the build process.

## Plugins Used

This project uses the following plugins:

1. **Java Plugin**: Adds support for Java projects.
2. **JUnit Platform Plugin**: Integrates JUnit 5 for unit testing.

## Build the Project

### Prerequisites

- **Java Development Kit (JDK) 8 or higher**: Ensure that the JDK is installed and configured in your environment.
- **Gradle**: This project uses Gradle as the build tool.

### Steps to Build

To build the project, follow these steps:

1. **Clone the repository**:
```shell
git clone git@github.com:ruslanaprus/goit-academy-dev-hw01-gradle.git
cd goit-academy-dev-hw01-gradle
```
2. **Build the project**:
```shell
gradle build
```

This command compiles the source code, runs the tests, and packages the application into a fat JAR file named `myname.jar` located in the `build/libs` directory. The fat JAR will include all dependencies, making it easier to distribute and run the application without needing to manage the classpath.

### Running the Application
After creating the fat JAR, you can run the application using the following command:
```shell
java -jar build/libs/myname.jar
```

This will execute the main method in `NameApp.java`, and you should see the serialized JSON string printed in the console.
