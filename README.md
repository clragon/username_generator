# username_gen

## Random username generator

This is a simple package to create random usernames. To user it simply make these commands, ported from [Javascript]('https://github.com/MaPhil/username-generator/')

```dart
import 'package:username_gen/username_gen.dart';

var username = UsernameGen.gen();

 //OR

final username = UsernameGen().generate();

```

If you want to set an array of name (nouns) and or adjectives use these commands and also if you want to use a different seperator commands

```dart

import 'package:username_gen/username_gen.dart';

final username = UsernameGen.gen(
    data: UsernameGenData(
        names: ['new names'],
        adjectives: ['new adjectives'],
    ),
    seperator: '_'
);

 //OR

final username = UsernameGen()
      ..setNames(['new names'])
      ..setSeperator('_')
      ..setAdjectives(['new adjectives'])
      ..generate();
```
