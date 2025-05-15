# Flutter GitHub Actions Sample

This is a sample Flutter project that demonstrates how to set up GitHub Actions for continuous integration.

## CI/CD Pipeline

The project uses GitHub Actions to:
- Run tests
- Check code formatting
- Analyze code
- Build for Android and iOS

### Workflow Details

The CI pipeline runs on:
- Push to main branch
- Pull requests to main branch

It includes the following jobs:
1. **Test Job**
   - Runs on Ubuntu
   - Installs dependencies
   - Verifies code formatting
   - Analyzes code
   - Runs tests

2. **Android Build Job**
   - Runs after tests pass
   - Builds debug APK

3. **iOS Build Job**
   - Runs after tests pass
   - Builds debug iOS app (without code signing)

## Local Development

To run the project locally:

```bash
# Install dependencies
flutter pub get

# Run tests
flutter test

# Format code
dart format .

# Analyze code
flutter analyze

# Run the app
flutter run
```

## Requirements

- Flutter SDK: ^3.19.3
- Dart SDK: ^3.7.2

## License

This project is open source and available under the MIT License.
