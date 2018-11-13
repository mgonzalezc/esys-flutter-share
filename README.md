# esys_flutter_share

A flutter plugin (iOS & Android) for sharing images with other applications.

## Installation
Add the following lines to the dependencies in the pubspec.yaml file:

```yaml
esys_flutter_share:
     git:
       url: git@github.com:esysberlin/esys-flutter-share.git
```

## Usage
Import:

```dart
import 'package:esys_flutter_share/esys_flutter_share.dart';
```

Share an image:

```dart
final ByteData bytes = await rootBundle.load('assets/image.png');
EsysFlutterShare.shareImage('myImageTest.png', 'myTitle', bytes);
```