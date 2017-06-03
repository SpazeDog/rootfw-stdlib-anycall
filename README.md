RootFW stdLib Anycall
=============

Anycall binaries for rootfw-stdlib

These binaries are used with the `SystemService` class in `rootfw-stdlib`. They are added to a separate package as to limit the size of `rootfw-stdlib`. There is no need to pack binaries if they are never being used. If anyone wishes to use this class, they can include this package. You can also compile your own from the source at [dk-zero-cool/anycall-native](https://github.com/dk-zero-cool/anycall-native) and add it to your own package `asset/` folder.

### Include Library
-----------

**Maven**

Reflect Tools is available in Maven respository at [Bintray](https://bintray.com/dk-zero-cool/maven/rootfw-stdlib-anycall/view) and can be accessed via jCenter.

```
dependencies {
    compile 'com.spazedog.lib.rootfw:rootfw-stdlib-anycall:$version'
}
```

**Android Studio**

First download the [rootfw-stdlib-anycall-release.aar](https://github.com/SpazeDog/rootfw-stdlib/raw/master/releases/rootfw-stdlib-anycall-release.aar) file.

Place the file in something like the `libs` folder in your module.

Open your `build.gradle` file for your module _(not the main project version)_.

```
dependencies {
    compile(name:'rootfw-stdlib-anycall-release', ext:'aar')
}

repositories {
    flatDir {
        dirs 'libs'
    }
}
```

