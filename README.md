# App de superhéroes

Aplicación Android de práctica construida con Kotlin, Jetpack Compose y Material 3. Presenta seis superhéroes en una lista desplazable, con ilustración, nombre y descripción. Incluye tipografía Cabin, barra superior centrada, tarjetas con elevación y esquinas redondeadas, diseño adaptable a tema claro u oscuro y configuración edge-to-edge.

## Abrir y ejecutar en Android Studio

1. Instala Android Studio y un JDK 17 o posterior. El proyecto apunta al SDK 35 y funciona desde Android 7.0 (API 24).
2. Clona esta repo:

   ```bash
   git clone https://github.com/ElkinDelgado25/superheroes-compose-uleam.git
   ```

3. En Android Studio, selecciona **Open** y elige la carpeta `SuperheroesComposeMoodle` del clon.
4. Espera a que termine **Gradle Sync** y acepta la instalación del SDK 35 si Android Studio la solicita.
5. Selecciona un emulador o conecta un dispositivo con Android 7.0 o posterior.
6. Pulsa **Run**. También puedes generar el APK de depuración con `./gradlew assembleDebug` desde la carpeta del proyecto.

## Cómo está organizada

- `model/Hero.kt` define el modelo de datos de un héroe.
- `model/HeroesRepository.kt` reúne los seis elementos que aparecen en la app.
- `HeroesScreen.kt` construye cada tarjeta y la lista con `LazyColumn`.
- `SuperheroesApp.kt` organiza la barra superior y la pantalla dentro de `Scaffold`.
- `ui/theme/` contiene la paleta, las formas, la tipografía Cabin y la configuración edge-to-edge.
- `res/drawable/`, `res/font/` y `res/values/` contienen ilustraciones, fuentes y textos.

## Pasos de la práctica

1. Crea el proyecto **Empty Activity** con Compose y minSdk 24.
2. Declara los recursos de héroes en `strings.xml` y crea la clase `Hero` con referencias a texto e imagen.
3. Organiza los seis registros en `HeroesRepository`.
4. Añade los colores Material 3, las formas redondeadas y la familia tipográfica Cabin.
5. Implementa una tarjeta de 72 dp para la ilustración, con esquinas de 8 dp, junto al nombre y la descripción.
6. Muestra las tarjetas en una `LazyColumn` y añade la barra superior centrada mediante `Scaffold`.
7. Configura los colores de la barra de estado y navegación para soportar edge-to-edge y tema oscuro.
8. Ejecuta la app en un emulador o dispositivo y revisa el desplazamiento y la legibilidad en ambos temas.

## Recursos y licencias

La estructura y los recursos gráficos y tipográficos de la práctica se basan en el repositorio oficial de entrenamiento de Android: [Basic Android Kotlin Compose Training: Superheroes](https://github.com/google-developer-training/basic-android-kotlin-compose-training-superheroes). Las ilustraciones están bajo Apache 2.0 y los archivos Cabin bajo SIL Open Font License 1.1, según `ASSETS_LICENSE.txt`. El código de esta práctica se distribuye bajo Apache 2.0; consulta `LICENSE`.
