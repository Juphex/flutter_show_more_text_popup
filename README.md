# flutter_show_widget_popup with dynamic height and width

Flutter widget to show widgets in popup or overlay container.
This fork has removed the Text widget and replaced it with a general Widget, thus any widget can be displayed.

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
The opacity parameter determines wether the widget has transparency.

```dart
import 'package:show_more_text_popup/show_more_text_popup.dart';
```


```dart
ShowMoreTextPopup popup = ShowMoreTextPopup(context,
       widget: Text(
          text,
          overflow: TextOverflow.clip,
          style: TextStyle(color: Colors.black),
          maxLines: 10,
        ),
        height: 10,
        width: 150,
        backgroundColor: backgroundColorStart,
        padding: EdgeInsets.all(10.0),
        borderRadius: BorderRadius.circular(10.0),
        opacity: 0.9,
        vsync: this
);

popup.show(
  widgetKey: key,
);
```

## Screenshots
<img src="https://raw.githubusercontent.com/snj07/flutter_show_more_text_popup/master/screenshots/show_more_text_popup_demo.gif" width="250" />
