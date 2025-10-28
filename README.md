# What is Flutter?

`Introduction to Flutter`: Flutter is an open-source UI software development kit (SDK) by Google that allows developers to create high-performance, natively compiled applications for mobile, web, and desktop from a single codebase. By using Flutter, developers can simplify app development with a unified framework that works across different platforms, reducing the complexity and time involved in managing multiple codebases.

## Architecture of Flutter:

- `Flutter Framework:` Built using the Dart programming language, Flutter is centered around a widget-based architecture. In Flutter, everything is a widget, from basic UI elements like buttons to entire screens. These widgets are highly customizable and reusable, allowing developers to efficiently build consistent user interfaces across platforms.
- `Rendering Engine:` Flutter uses `Impeller rendering engine`. Impeller precompiles a smaller, simpler set of shaders at Engine-build time so they don't compile at runtime.

## Benefits of Flutter:

- `Hot Reload:` One of Flutter’s most powerful features is hot reload, which allows developers to instantly see the effects of code changes without restarting the entire app. This feature speeds up development by enabling quick iterations and experimentation.
- `Single Codebase:` Flutter enables developers to maintain a single codebase that can be used to create apps for multiple platforms, including Android, iOS, web, and desktop. This significantly reduces development time and costs.
- `Rich Set of Widgets:` Flutter comes with a comprehensive library of pre-designed widgets that are both beautiful and customizable. These widgets adhere to the design guidelines of both Android (Material Design) and iOS (Cupertino), ensuring that apps built with Flutter provide a native-like experience on each platform.

`Real-World Applications:` Some popular applications built with Flutter include the Google Ads app, Reflectly, and Alibaba. These apps benefit from Flutter’s rapid development cycles and consistent performance across platforms.

## Key Points:

- Flutter is a versatile and powerful framework for cross-platform development.
- It uses a single codebase for multiple platforms, making it an efficient tool for developers.
- Flutter’s architecture revolves around widgets, with hot reload enabling quick iterations and testing.

# What are Widgets?

Widgets are the `building blocks` of a Flutter app's user interface. In Flutter, everything you see on the screen is a widget, whether it’s a `text`, `image`, or `button`. Even structural elements like `rows`, `columns`, and `layouts` are widgets.

Flutter uses a `widget tree` to determine how widgets are arranged and displayed. Widgets are lightweight and designed to be `reusable`.

## Types of Widgets

Flutter provides two main types of widgets based on their state:

### 1. StatelessWidget

- These widgets are `immutable`, meaning their state cannot change after they are built.

- Examples: `Text`, `Icon`, `AppBar`.

- Use when the UI remains static.

### 2. StatefulWidget

- These widgets are `mutable`, meaning they can change their state during runtime.

- Examples: `Checkbox`, `Slider`, `TextField`.

- Use when the UI needs to update dynamically based on user interactions or data changes.

## Building a Simple UI with Widgets:

By combining different widgets, you can build complex UIs. For example:

- Use a `Column` widget to arrange a group of widgets vertically.
- Wrap a `Text` widget inside a `Padding` widget to add space around the text. 
- Place a `Button` widget within a `Container` to style it with background color, padding, and borders.

### Key Takeaways

- Widgets are `reusable` components that build the Flutter UI.

- Use `StatelessWidget` for static UI elements.

- Use `StatefulWidget` for interactive or dynamic UI elements.

- Familiarize yourself with common widgets like `Text`, `Container`, `Buttons`, and `Lists`, as they form the core of most Flutter apps.

# Flutter Widgets — Complete Reference Table

## Basic Widgets
| Widget | Use / Description |
|--------|--------------------|
| `Text` | Displays a string of text. |
| `RichText` | Displays text with multiple styles (colors, fonts, etc.). |
| `Image` | Displays an image (from asset, file, or network). |
| `Icon` | Displays a Material Design icon. |
| `Container` | A styled box for layout (color, padding, margin, etc.). |
| `SizedBox` | Creates fixed-size boxes or spacing. |
| `Spacer` | Adds flexible space between widgets in Row/Column. |
| `Center` | Centers its child. |
| `Padding` | Adds space around its child. |
| `Align` | Aligns child within itself. |
| `FittedBox` | Scales and positions its child. |
| `Divider` | Draws a horizontal dividing line. |

## Layout Widgets
| Widget | Use / Description |
|--------|--------------------|
| `Row` | Lays out children horizontally. |
| `Column` | Lays out children vertically. |
| `Stack` | Overlaps widgets (Z-axis). |
| `Expanded` | Fills remaining space in Row/Column. |
| `Flexible` | Like Expanded with flexible sizing. |
| `Wrap` | Wraps children to next line. |
| `Flow` | Manual widget positioning (advanced). |
| `GridView` | Grid layout of widgets. |
| `ListView` | Scrollable vertical list. |
| `SingleChildScrollView` | Makes a single child scrollable. |
| `Table` | Displays children in rows/columns. |
| `CustomScrollView` | Custom scroll effects with slivers. |
| `SliverList / SliverGrid` | Efficient scrolling lists/grids. |

## Input & Interaction
| Widget | Use / Description |
|--------|--------------------|
| `TextField` | User text input. |
| `Form` | Groups form fields with validation. |
| `FormField` | Base for form inputs. |
| `Checkbox` | True/false input selection. |
| `Radio` | Select one value from many. |
| `Switch` | Toggle on/off. |
| `Slider` | Select value by sliding. |
| `DropdownButton` | Dropdown selection. |
| `GestureDetector` | Detects taps, swipes, drags. |
| `InkWell` | Touch ripple effect. |
| `ElevatedButton` | Raised button with elevation. |
| `TextButton` | Flat text button. |
| `OutlinedButton` | Button with outline border. |
| `IconButton` | Icon-only button. |
| `FloatingActionButton` | Floating circular button. |
| `ToggleButtons` | Group of toggleable buttons. |

## Styling & Theming
| Widget | Use / Description |
|--------|--------------------|
| `Theme` | Defines colors, fonts, shapes. |
| `ColorFiltered` | Applies color filter. |
| `DecoratedBox` | Adds background, border, or shadow. |
| `Opacity` | Adjusts transparency. |
| `ShaderMask` | Applies gradient or shader. |

## Image & Media
| Widget | Use / Description |
|--------|--------------------|
| `Image.asset` | Loads image from assets. |
| `Image.network` | Loads image from internet. |
| `Image.file` | Loads image from filesystem. |
| `FadeInImage` | Placeholder while loading image. |
| `VideoPlayer` | Plays video. |
| `CircleAvatar` | Circular profile image/initials. |

## Navigation Widgets
| Widget | Use / Description |
|--------|--------------------|
| `Navigator` | Manages navigation stack. |
| `MaterialApp` | Root Material app widget. |
| `CupertinoApp` | Root iOS-style app widget. |
| `Scaffold` | Page structure (app bar, drawer). |
| `AppBar` | Header bar with title/actions. |
| `Drawer` | Side navigation menu. |
| `BottomNavigationBar` | Bottom navigation tabs. |
| `TabBar / TabBarView` | Tab navigation. |
| `PageView` | Swipeable page switching. |

## State Management
| Widget | Use / Description |
|--------|--------------------|
| `StatefulWidget` | Maintains state across rebuilds. |
| `StatelessWidget` | No internal state. |
| `InheritedWidget` | Shares data down tree. |
| `Provider` (package) | Simple state management. |

## Animation Widgets
| Widget | Use / Description |
|--------|--------------------|
| `AnimatedContainer` | Animates size, color, etc. |
| `AnimatedOpacity` | Animates fade visibility. |
| `AnimatedPositioned` | Animates Stack position. |
| `AnimatedCrossFade` | Animates between two children. |
| `Hero` | Screen transition animations. |
| `FadeTransition` | Fade animation. |
| `ScaleTransition` | Scale animation. |
| `RotationTransition` | Rotate animation. |

## Advanced Layout
| Widget | Use / Description |
|--------|--------------------|
| `CustomPaint` | Draw custom shapes/graphics. |
| `ReorderableListView` | Drag-and-drop list reordering. |
| `LayoutBuilder` | Builds based on constraints. |
| `AspectRatio` | Enforces width/height ratio. |
| `FractionallySizedBox` | Sizes child by fraction. |
| `IntrinsicHeight / IntrinsicWidth` | Sizes to child’s natural dimensions. |

## Scrollable Widgets
| Widget | Use / Description |
|--------|--------------------|
| `ListView.builder` | Efficient on-demand list building. |
| `GridView.builder` | Efficient on-demand grid building. |
| `NestedScrollView` | Nested scrolling. |
| `Scrollbar` | Adds scrollbar indicator. |

## Dialogs & Notifications
| Widget | Use / Description |
|--------|--------------------|
| `AlertDialog` | Popup dialog with actions. |
| `SimpleDialog` | Basic options dialog. |
| `SnackBar` | Temporary bottom message. |
| `BottomSheet` | Panel sliding from bottom. |
| `Toast` (package) | Brief overlay message. |

## App Structure
| Widget | Use / Description |
|--------|--------------------|
| `MaterialApp` | Material design entry. |
| `CupertinoApp` | iOS entry. |
| `Scaffold` | Page layout. |
| `SafeArea` | Avoids system UI overlaps. |
| `WillPopScope` | Intercepts back button. |

## Data & Lists
| Widget | Use / Description |
|--------|--------------------|
| `FutureBuilder` | Builds from asynchronous data. |
| `StreamBuilder` | Builds from stream updates. |
| `ListTile` | Standard list item layout. |
| `DataTable` | Table of data. |
| `ExpansionTile` | Expandable list item. |

## Utility Widgets
| Widget | Use / Description |
|--------|--------------------|
| `Builder` | Generates a new BuildContext. |
| `MediaQuery` | Access screen size/orientation. |
| `Navigator` | Routing control. |
| `FutureBuilder` | Builds async data UI. |
| `StreamBuilder` | Live data UI builder. |

## Widget Classification Summary
| Type | Description |
|------|-------------|
| `StatelessWidget` | Does not hold internal state. |
| `StatefulWidget` | Holds changing state. |
| `InheritedWidget` | Efficient data sharing down tree. |
| `RenderObjectWidget` | Low-level custom rendering. |
