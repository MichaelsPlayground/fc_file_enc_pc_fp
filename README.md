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

build ios release
```plaintext
/Users/michaelfehr/flutter/bin/flutter build ios --release --no-codesign

```

```plaintext
I just wanted to build the ios .ipa file for the testing purpose without any hustle, follow are the step I took, and hopefully, they will be helpful.
In the terminal run this command.
  flutter build ios --release --no-codesign
After that go to the folder where the output is stored.
build/ios/iphoneos
After that you will have to create a new directory/folder in the iphoneos folder called "Payload".
After that move the output file "Runner.app" (name can be different) to the "Payload" folder.
Then compress the "Payload" folder and rename to "YouAppName.ipa". (make sure to change the extension)
And it's done.
The solution will help you get .ipa file without signing.
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
