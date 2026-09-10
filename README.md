# Bhaktiwala

Bhaktiwala is an Android app for keeping devotional experiences accessible from a mobile device.

## Repository Status

This repository currently contains an extracted Android application package rather than the original Android Studio project. It includes compiled bytecode, packaged resources, Kotlin metadata, and bundled Android/Firebase libraries.

Because the original source tree and Gradle build files are not included, this repository is not currently reproducible as a source build.

## What Is Included

- Android application manifest and packaged resources
- Compiled application bytecode in `classes.dex`
- Kotlin runtime metadata
- AndroidX and Material Components dependencies
- Firebase Authentication and Google identity dependencies
- Google Play services dependencies

## Installation

An APK file is required to install and run the app. The APK is not included in this repository.

Once an APK is available, it can be installed on a connected Android device with:

```bash
adb install path/to/bhaktiwala.apk
```

The device should have USB debugging enabled and allow installation from the connected computer.

## Development

To make Bhaktiwala buildable from source, add the original Android Studio project, including:

- Gradle wrapper and build configuration
- Application source code
- Resource XML and asset source files
- Firebase configuration appropriate for the target environment
- Signing configuration kept outside version control

Do not commit `google-services.json`, signing keys, API keys, or other environment-specific secrets to a public repository.

## Contributing

Issues and pull requests are welcome once the source project is added. Please include clear reproduction steps for bugs and keep credentials and private configuration out of commits.

## License

No license has been provided yet. Add a license before distributing or accepting external contributions.
