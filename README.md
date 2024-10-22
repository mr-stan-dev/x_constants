<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages).
-->

A Flutter package with a conveniently designed common constants for Flutter projects.

At the moment inludes 4 types of constants:
1. Border
2. Duration
3. Padding
4. Spacing

## Features

![x_const](https://github.com/user-attachments/assets/3e259799-885e-40e7-982d-21767663c3db)


## Getting started

In the `pubspec.yaml` of your flutter project, add the following dependency:

```yaml
dependencies:
  ...
  x_constants: ^0.0.1
```

Import it:

```dart
import 'package:x_constants/x_constants.dart';
```

## Usage

```dart
  @override
  Widget build(BuildContext context) {
    return Column(
      children: [
        Container(
          decoration: const BoxDecoration(
            borderRadius: XBorder.all16,
            color: Colors.yellow,
          ),
          child: const Padding(
            padding: XPadding.all16,
            child: Text('Text 1'),
          ),
        ),
        XSpacing.vertical16,
        const Padding(
          padding: XPadding.all16,
          child: Text('Text 2'),
        ),
      ],
    );
  }
```

## Additional information

Feel free to raise a PR, but make sure that new constants are commonly used.
