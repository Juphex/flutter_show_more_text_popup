# flutter_show_more_text_popup with dynamic height and width

Flutter widget to show text in popup or overlay container

## Installation

Add this to your package's pubspec.yaml file

```yaml
dependencies:
  ...
  show_more_text_popup: ^latest-version
```

## Usage
First import show_more_text_popup.dart
The given height and width are (partially-) ignored and calculated dynamically by flutter.

```dart
import 'package:show_more_text_popup/show_more_text_popup.dart';
```


```dart
ShowMoreTextPopup popup = ShowMoreTextPopup(context,
        text: text,
        textStyle: TextStyle(color: Colors.black),
        height: 200,
        width: 100,
        backgroundColor: Color(0xFF16CCCC),
        padding: EdgeInsets.all(4.0),
        borderRadius: BorderRadius.circular(10.0)
);

popup.show(
  widgetKey: key,
);
```

## Screenshots
<img src="https://raw.githubusercontent.com/snj07/flutter_show_more_text_popup/master/screenshots/show_more_text_popup_demo.gif" width="250" />
