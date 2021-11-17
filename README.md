# fc_file_enc_pc_fp

uses flutter file dialog for file choosing

uses pointycastle for aes gcm pbkdf2 file encryption

funktioniert unter iOS und unter Android

todo: delete files in app dir and cache dir

```plaintext
https://pub.dev/packages/pointycastle
pointycastle: ^3.4.0
https://github.com/bcgit/pc-dart

https://pub.dev/packages/path_provider
path_provider: ^2.0.7

https://pub.dev/packages/flutter_file_dialog
flutter_file_dialog: ^2.3.0
https://github.com/kineapps/flutter_file_dialog
```

in build.gradle (application)
```plaintext
defaultConfig {
    // TODO: Specify your own unique Application ID (https://developer.android.com/studio/build/application-id.html).
    applicationId "de.fluttercrypto.fc_file_enc_pc_fp"
    minSdkVersion 19
    targetSdkVersion 30
    versionCode flutterVersionCode.toInteger()
    versionName flutterVersionName
    }
```
in podfile:
```plaintext
# Uncomment this line to define a global platform for your project
platform :ios, '10.0'
```

```plaintext

```

```plaintext

```

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
