# Google Ads Mobile Flutter Integration

[![Build Status](https://github.com/Dimvy-Clothing-brand/googleads-mobile-flutter/actions/workflows/build.yaml/badge.svg?branch=nodoubtz-patch-1)](https://github.com/Dimvy-Clothing-brand/googleads-mobile-flutter/actions/workflows/build.yaml)

## Overview

This repository contains a Flutter integration for Google Ads Mobile. It provides a seamless way to integrate Google Ads into your Flutter mobile applications, allowing you to monetize your apps using Google's advertising platform.

## Features

- Easy integration of Google Ads in Flutter applications.
- Support for various ad formats including banner, interstitial, and rewarded ads.
- Customizable ad placements.
- Built-in support for ad lifecycle management.
- Comprehensive documentation and examples for quick setup and usage.

## Getting Started

Follow the instructions below to set up and use this package in your Flutter project.

### Prerequisites

- Flutter SDK 2.0 or higher
- Dart 2.12 or higher
- Google Ads account
- Ensure your app is registered in the Google AdMob platform

### Installation

Add the package to your `pubspec.yaml` file:

```yaml
dependencies:
  googleads_mobile_flutter: ^1.0.0
```

Then, run the following command to fetch the package:

```bash
flutter pub get
```

### Usage

1. **Configure AdMob in your Flutter Project:**

   Add your AdMob app ID to your `AndroidManifest.xml` and `Info.plist` files for Android and iOS, respectively.

2. **Initialize the Google Ads SDK:**

   Call the initialization method in your app's `main` function:

   ```dart
   void main() async {
     WidgetsFlutterBinding.ensureInitialized();
     await GoogleAdsMobileFlutter.initialize();
     runApp(MyApp());
   }
   ```

3. **Display Ads:**

   Use the provided widgets or APIs to display ads in your app. For example:

   ```dart
   BannerAd(
     adUnitId: 'your-ad-unit-id',
     size: AdSize.banner,
   )
   ```

Refer to the detailed documentation in the `docs` folder for additional features and examples.

## Contributing

We welcome contributions to enhance this project. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and push them to your fork.
4. Submit a pull request with a detailed description of your changes.

## Build and Test

This project uses GitHub Actions for continuous integration. The current build status is displayed above. To run tests locally, use the following command:

```bash
flutter test
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or support, please reach out to the project maintainers through [GitHub Issues](https://github.com/Dimvy-Clothing-brand/googleads-mobile-flutter/issues).

---
Happy coding! 🚀
