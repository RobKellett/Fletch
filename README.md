# Fletch [![Build Status](https://drone.io/github.com/RobKellett/Fletch/status.png)](https://drone.io/github.com/RobKellett/Fletch/latest)
### jQuery for Dart

Fletch is a [Dart](https://www.dartlang.org/) library aiming to provide similar
functionality to [jQuery](http://jquery.com/). However, Fletch is _not_
designed to be API-compatible with jQuery, instead preferring to take advantage
of Dart features and design patterns.

For example, here is a snippet of jQuery:
```javascript
$("<a>").text("Dart is cool!")
        .attr("href", "https://www.dartlang.org/")
        .style("font-weight", "bold")
        .appendTo("body");
```

Here is the equivalent code in Fletch:
```dart
$("<a>")..text = "Dart is cool!"
        ..attr["href"] = "https://www.dartlang.org/"
        ..style["font-weight"] = "bold"
        ..appendTo("body");
```

Full API documentation is available [here](http://robkellett.github.io/Fletch/).

Fletch is very much a work in progress. So far, Fletch supports the most common
cases for manipulating the DOM, styles, attributes, events, and form data.
Fletch should be considered **alpha quality**, as the public-facing API may 
change radically between releases.

## Installing

[Fletch is available on **pub**.](http://pub.dartlang.org/packages/fletch) Add
"fletch" as a dependency and run `pub install`. Then, just import Fletch into
your code with `import 'package:fletch/fletch.dart';` and you're all set!

Fletch is released under the **ISC License**, which is functionally equivalent
to the BSD-2 and MIT licenses. See the `LICENSE` file for more information.