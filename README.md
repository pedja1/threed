# Threed

[![JitPack](https://jitpack.io/v/samelody/threed.svg)](https://jitpack.io/#samelody/threed)
![Android](https://img.shields.io/badge/platform-Android-brightgreen.svg)
[![Apache](https://img.shields.io/hexpm/l/plug.svg)](LICENSE)
![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg)

MoreTextView for Android. Click the TextView to show more text.

**DO NOT USE THIS LIBRARY IN PRODUCTION** until `1.0.0` is released.

# Screenshot

<img src="./art/sample.gif" style="width:300px;height:500px;" />

# Download

This project is available on `JitPack` repository.

In your root `build.gradle`:

```gradle
allprojects {
    repositories {
        // ...
        maven { url "https://jitpack.io" }
    }
}
```

In your app `build.gradle`:

```gradle
dependencies {
    compile 'com.github.samelody:threed:0.1.1'
}
```

# Getting started

Add `MoreTextView` into your UI layout:

```xml
<com.samelody.threed.MoreTextView
    android:id="@+id/text2"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:maxLines="2"
    android:text="@string/your_text"
    app:moreText="@string/more"
    app:moreTextColor="@color/moreColor"
    />
```

Setup a `OnEllipsizeChangeListener`:

```java
Threed.setOnEllipsizeChangeListener(moreTextView, onEllipsizeChangeListener);
```

# Dependencies

```java
compile 'com.android.support:appcompat-v7:25.3.0'
```

# Compatibility

- **Android SDK**: Requires a minimum API level of 14.

# License

    Copyright (c) 2017-present Samelody.com

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.