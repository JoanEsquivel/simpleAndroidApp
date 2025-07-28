# Simple Android App - Test Automation

## Descripción del Proyecto

Este es un proyecto de Android simple que demuestra la implementación de tests unitarios usando la librería Truth de Google. El proyecto incluye una clase `Tax` para cálculos de impuestos y tests unitarios correspondientes.

## Características Principales

### MainActivity
La actividad principal (`MainActivity.kt`) contiene:
- Inicialización de la clase `Tax`
- Cálculo de ingresos netos y impuestos
- Ejecución de cálculos de ejemplo con valores de prueba

```kotlin
val tax = Tax()
val netIncome = tax.calculateIncome(100.0, 0.1)
val netTax = tax.calculateTax(100.0, 0.1)
```

### Clase Tax
La clase `Tax` (`Tax.kt`) proporciona dos métodos principales:
- `calculateTax()`: Calcula el monto de impuestos basado en ingresos brutos y tasa de impuesto
- `calculateIncome()`: Calcula el ingreso neto después de impuestos

### Tests Unitarios
Los tests unitarios (`TestTax.kt`) utilizan la librería **Truth** de Google para assertions más legibles:
- Test para cálculo de impuestos
- Test para cálculo de ingresos netos
- Uso de assertions fluidas con Truth

## Requerimientos del Sistema

### Requisitos Mínimos
- **Android SDK**: API Level 23 (Android 6.0 Marshmallow)
- **Target SDK**: API Level 32 (Android 12)
- **Java**: Versión 1.8
- **Kotlin**: Versión 1.7.10
- **Gradle**: Versión 7.2.2

### Dependencias Principales
- **AndroidX Core**: 1.7.0
- **AndroidX AppCompat**: 1.3.0
- **Material Design**: 1.4.0
- **JUnit**: 4.13.2
- **Truth**: 1.4.4 (para assertions fluidas)

## Configuración del Proyecto

### Prerrequisitos
1. Android Studio (versión recomendada: Arctic Fox o superior)
2. JDK 8 o superior
3. Android SDK con API Level 23-32

### Instalación
1. Clona el repositorio
2. Abre el proyecto en Android Studio
3. Sincroniza el proyecto con Gradle
4. Ejecuta los tests unitarios para verificar la configuración

## Ejecutar Tests

Para ejecutar los tests unitarios:
```bash
./gradlew test
```

O desde Android Studio:
- Navega a `app/src/test/java/com/joanmedia/testintro/TestTax.kt`
- Haz clic derecho en la clase y selecciona "Run 'TestTax'"

## Estructura del Proyecto

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

## Tecnologías Utilizadas

- **Kotlin**: Lenguaje de programación principal
- **AndroidX**: Librerías de soporte de Android
- **JUnit**: Framework de testing
- **Truth**: Librería de assertions fluidas de Google
- **Gradle**: Sistema de build

## Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.
