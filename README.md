# Flutter Restoration Mixin Example

This project demonstrates the use of the `RestorationMixin` in a Flutter application.
The `RestorationMixin` allows the state of a widget to be restored when the app is restarted.

## Documentation
- [Flutter Documentation- State Restoration on android](https://docs.flutter.dev/platform-integration/android/restore-state-android)
- [RestorationMixin](https://api.flutter.dev/flutter/widgets/RestorationMixin-mixin.html)

## Getting Started

### Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- [Dart SDK](https://dart.dev/get-dart)

### Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/praharshbhatt/flutter_restorationmixin_example.git
    cd flutter_restorationmixin_example
    ```

2. **Install dependencies:**

    ```sh
    flutter pub get
    ```

3. **Run the app:**

    ```sh
    flutter run
    ```

## Project Structure

- `lib/main.dart`: Contains the main application code, including the `RestorableCounter` widget
  which uses the `RestorationMixin` to restore its state.
- `test/widget_test.dart`: Contains widget tests to verify the functionality of
  the `RestorableCounter` widget.

## Code Overview

### `RestorationExampleApp`

A simple `StatelessWidget` that sets up the `MaterialApp` with a `RestorableCounter` as the home
widget.

### `RestorableCounter`

A `StatefulWidget` that uses the `RestorationMixin` to save and restore the state of a counter.

### `_RestorableCounterState`

The state class for `RestorableCounter` that implements the `RestorationMixin`. It uses
a `RestorableInt` to store the counter value.

## Running Tests

To run the widget tests, use the following command:

```sh
flutter test
```

## Example Tests

The project includes tests to verify the functionality of the `RestorableCounter` widget:

- **Counter increments smoke test:** Verifies that the counter increments correctly.
- **Counter value is restored:** Verifies that the counter value is restored correctly after a
  simulated app restart.

## Resources

- [Flutter Documentation](https://flutter.dev/docs)
- [Dart Documentation](https://dart.dev/guides)
- [RestorationMixin API](https://api.flutter.dev/flutter/widgets/RestorationMixin-class.html)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug
fixes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.