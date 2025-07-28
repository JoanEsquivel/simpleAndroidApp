# Simple Android App - Test Automation

## Project Description

This is a simple Android project that demonstrates the implementation of unit tests using Google's Truth library. The project includes a `Tax` class for tax calculations and corresponding unit tests.

## Main Features

### MainActivity
The main activity (`MainActivity.kt`) contains:
- Initialization of the `Tax` class
- Calculation of net income and taxes
- Execution of example calculations with test values

```kotlin
val tax = Tax()
val netIncome = tax.calculateIncome(100.0, 0.1)
val netTax = tax.calculateTax(100.0, 0.1)
```

### Tax Class
The `Tax` class (`Tax.kt`) provides two main methods:
- `calculateTax()`: Calculates tax amount based on gross income and tax rate
- `calculateIncome()`: Calculates net income after taxes

### Unit Tests
The unit tests (`TestTax.kt`) use Google's **Truth** library for more readable assertions:
- Test for tax calculation
- Test for net income calculation
- Use of fluent assertions with Truth

## System Requirements

### Minimum Requirements
- **Android SDK**: API Level 23 (Android 6.0 Marshmallow)
- **Target SDK**: API Level 32 (Android 12)
- **Java**: Version 1.8
- **Kotlin**: Version 1.7.10
- **Gradle**: Version 7.2.2

### Main Dependencies
- **AndroidX Core**: 1.7.0
- **AndroidX AppCompat**: 1.3.0
- **Material Design**: 1.4.0
- **JUnit**: 4.13.2
- **Truth**: 1.4.4 (for fluent assertions)

## Project Setup

### Prerequisites
1. Android Studio (recommended version: Arctic Fox or higher)
2. JDK 8 or higher
3. Android SDK with API Level 23-32

### Installation
1. Clone the repository
2. Open the project in Android Studio
3. Sync the project with Gradle
4. Run unit tests to verify the configuration

## Running Tests

To run unit tests:
```bash
./gradlew test
```

Or from Android Studio:
- Navigate to `app/src/test/java/com/joanmedia/testintro/TestTax.kt`
- Right-click on the class and select "Run 'TestTax'"

## Project Structure

```
app/
├── src/
│   ├── main/
│   │   ├── java/com/joanmedia/testintro/
│   │   │   ├── MainActivity.kt
│   │   │   └── Tax.kt
│   │   └── res/
│   └── test/
│       └── java/com/joanmedia/testintro/
│           └── TestTax.kt
└── build.gradle
```

## Technologies Used

- **Kotlin**: Main programming language
- **AndroidX**: Android support libraries
- **JUnit**: Testing framework
- **Truth**: Google's fluent assertions library
- **Gradle**: Build system

## Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is under the MIT License. See the `LICENSE` file for more details.
