# Code Challenge

## Table of Contents

- [Summary](#summary)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Authors](#authors)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Summary
This project showcases the integration of Spring Batch and Spring Boot to process and serve data. It is organized into two subprojects:

- **ChallengeBatch**: a Spring Batch application.
- **ChallengeMS**: a Spring Boot microservice.

Follow the instructions below to set up and run the applications.

## Prerequisites

- Java 21
- Maven 3.9+

## Getting Started

To get started, follow these steps:

### Using IntelliJ IDEA

1. Clone the repository.
2. Open the project in IntelliJ IDEA.
3. Press 'Run' on the respective main class of each subproject:
   - Run **ChallengeBatch** first to initiate the batch processing.
   - Once **ChallengeBatch** has completed, a folder named `DB` will be created at the project root. This folder will contain an H2 database file from which the microservice will retrieve data.
   - Run **ChallengeMS** to start the microservice.

### Using Command Line

Alternatively, you can use Maven to compile the JAR files and run them from the command line:

```shell
# Run ChallengeBatch
cd ChallengeBatch
mvn clean install
java -jar target/batch-1.0-SNAPSHOT.jar

# Start ChallengeMS after running batch
cd ../ChallengeMS
mvn clean install
java -jar target/ms-1.0-SNAPSHOT.jar
```

## Authors

  - **Giovanbattista Abbate** - [giabb](https://github.com/giabb)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- **Billie Thompson** - *Provided README Template* - [PurpleBooth](https://github.com/PurpleBooth)