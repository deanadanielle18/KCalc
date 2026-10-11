# KCalc
Yet another calculator based on BODMAS rule :)

## Features
- Ability to evaluate and execute basic mathematical expressions.
- / ,  * , + , - are supported at the moment.
- Calculation history

## Approach
![Aproac](https://raw.githubusercontent.com/kdkanishka/KCalc/master/docs/images/1633417868332.jpg)

## Design
- Applied strategy pattern to implement open-closed principal

#### Core design
![Core Design](https://raw.githubusercontent.com/kdkanishka/KCalc/master/docs/images/kcalc.png)


## Implementation
- The application and core algorithm is implemented in java
- No external dependencies used for expression evaluation
- Java Swing is used to implement the simple calculator UI
- JUnit 5 for unit tests
- JaCoCo for coverage reports

## Screenshots
#### Expression evaluation & history
![screenshot 1](https://raw.githubusercontent.com/kdkanishka/KCalc/master/docs/images/Screenshot_20211005_115355.png)

#### Handling bad expressions
![screenshot 2](https://raw.githubusercontent.com/kdkanishka/KCalc/master/docs/images/Screenshot_20211005_115603.png)
## Requirements
- Java 11 or Higher
- Apache Maven 3.x
- Git (Optional) for cloning. (or direct download sources from github)

## Getting started
- Clone the project

`git clone https://github.com/kdkanishka/KCalc.git`

- Execute (Start the application without creating an executable jar)

`mvn compile exec:java -Dexec.mainClass="com.kani.kcalc.core.Main"`

- Run tests with test coverage

`mvn clean test`

- Coverage reports can be found on

`<PROJECT_DIR>/target/site/jacoco/index.html`

## Continuous Integration

This project uses GitHub Actions for continuous integration.

The CI workflow automatically runs the Maven test suite whenever changes
are pushed to the repository or a pull request is created.

The workflow performs the following steps:

1. Checks out the repository.
2. Sets up Java 11.
3. Runs the JUnit 5 tests using Maven.
4. Generates the JaCoCo coverage report.

The workflow configuration is located in:

`.github/workflows/maven.yml`

## Testing

The project includes JUnit 5 tests using black-box and white-box testing,
boundary value analysis, equivalence partitioning, path-based testing,
and data-flow testing.

## Author
Kanishka Dilshan (kdkanishka@gmail.com)
