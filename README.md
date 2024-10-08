# Circle Nav Bar

![](doc/animation.gif)

## Example style:

<table>
    <thead>
        <tr>
            <th><strong>no padding black</strong></th>
            <th><strong>padding with gradient</strong></th>
            <th><strong>Level and Icons</strong></th>
            <th><strong>only Icons </strong></th>
            <th><strong>padding with Levels and icons</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><img src="doc/nopadding-black.png" alt=""></td>
            <td><img src="doc/padding-gradient2.png" alt=""></td>
            <td><img src="doc/bottom-nev-with-levels.png" alt=""></td>
            <td><img src="doc/bottom-nev.png" alt=""></td>
            <td><img src="doc/floating-bottom-navbar.png" alt=""></td>
            
        </tr>
    </tbody>
</table>

## How to use

```yaml
dependencies:
  circle_nav_bar: ^latest_version
```

```dart
import 'package:circle_nav_bar/circle_nav_bar.dart';

Scaffold(
      bottomNavigationBar: CircleNavBar(
        activeIcons: const [
          Icon(Icons.person, color: Colors.deepPurple),
          Icon(Icons.home, color: Colors.deepPurple),
          Icon(Icons.favorite, color: Colors.deepPurple),
        ],
        inactiveIcons: const [
          Text("My"),
          Text("Home"),
          Text("Like"),
        ],
        color: Colors.white,
        circleColor: Colors.white,
        height: 60,
        circleWidth: 60,
        initIndex: 1,
        onChanged: (v) {
          // TODO
        },
        // tabCurve: ,
        padding: const EdgeInsets.only(left: 16, right: 16, bottom: 20),
        cornerRadius: const BorderRadius.only(
          topLeft: Radius.circular(8),
          topRight: Radius.circular(8),
          bottomRight: Radius.circular(24),
          bottomLeft: Radius.circular(24),
        ),
        shadowColor: Colors.deepPurple,
        circleShadowColor: Colors.deepPurple,
        elevation: 10,
        gradient: LinearGradient(
            begin: Alignment.topRight,
            end: Alignment.bottomLeft,
            colors: [ Colors.blue, Colors.red ],
        ),
        circleGradient: LinearGradient(
            begin: Alignment.topRight,
            end: Alignment.bottomLeft,
            colors: [ Colors.blue, Colors.red ],
        ),
      ),
      ...
```

![](doc/value.png)

![](doc/value-05.png)

![](doc/bottom-nev-with-levels.png)

![](doc/bottom-nev.png)

![](doc/floating-bottom-navbar.png)

### Now User Can Add Levels

### Active and inactive levels TextStyle are available.

### Hight set to Default. user can change as They need.

### circleWidth set to Default. user can change as They need.

### shadowColor and circleShadowColor is transparent as Default. user can change as They need.
