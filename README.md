# trees

A dart library for working with tree structures.

## Features

- Support for general trees
- bfs and dfs traversal

## Getting started

To use this package, add `trees` as a [dependency in your pubspec.yaml file](https://flutter.dev/docs/development/packages-and-plugins/using-packages).

```yaml
dependencies:
  trees: ^1.0.0
```

Import the package in your code:

```dart
import 'package:trees/trees.dart';
```

## Usage

An example of creating a tree and traversing it:

```dart
final root = GeneralTreeNode('root');
root.addChild('child1');
root.addChild('child2');

root.currentChild!.addChild('grandchild1');
root.currentChild!.addChild('grandchild2');

root.currentChild!.nextChild();

root.currentChild!.currentChild!.addChild('great-grandchild1');

print(root.chainData); // [root, child2]
```

## License

```
MIT License

Copyright (c) 2025 Dane Madsen

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
