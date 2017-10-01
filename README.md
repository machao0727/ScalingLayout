# ScalingLayout
Scale your layout on user interaction. [Live Demo](https://www.youtube.com/watch?v=wA41H0UMoHQ)

<img src="https://raw.githubusercontent.com/iammert/ScalingLayout/master/art/cover_scaling.png"/>

## Demo
<img src="https://github.com/iammert/ScalingLayout/blob/master/art/gif_coordinator.gif"/>

## Usage
```xml
<iammert.com.view.scalinglib.ScalingLayout
        android:id="@+id/scalingLayout"
        android:layout_width="300dp"
        android:layout_height="48dp"
        app:radiusFactor="1">
        
        <!-- Your content here -->
        
</iammert.com.view.scalinglib.ScalingLayout>
```

```java
scalingLayout.expand(); //use this if you want to expand all
scalingLayout.collapse(); //user this if you want to collapse view to initial state.
scalingLayout.setProgress(float progress); //1 is fully expanded, 0 is initial state.
```

## Listener
```java
scalingLayout.setListener(new ScalingLayoutListener() {
    @Override
    public void onCollapsed() {}

    @Override
    public void onExpanded() {}

    @Override
    public void onProgress(float progress) {}
});
```

## Attribute
```app:radiusFactor``` value is between 0 and 1 float value. 1 = full rounded corner. 0 = no rounded corner.

## ScalingLayoutBehaviour
<img src="https://github.com/iammert/ScalingLayout/blob/master/art/gif_behavior.gif"/>

```xml
<iammert.com.view.scalinglib.ScalingLayout
        android:id="@+id/scalingLayout"
        android:layout_width="300dp"
        android:layout_height="48dp"
        app:radiusFactor="1"
        app:layout_behavior="iammert.com.view.scalinglib.ScalingLayoutBehavior">
        
        <!-- Your content here -->
        
</iammert.com.view.scalinglib.ScalingLayout>
```

## Demos
* Spotify Search
<img src="https://github.com/iammert/ScalingLayout/blob/master/art/gif_searchbar.gif"/>

* Fab filter
<img src="https://github.com/iammert/ScalingLayout/blob/master/art/gif_fab.gif"/>

## Dependency
```gradle
  maven { url 'https://jitpack.io' }
```

```gradle
dependencies {
  compile 'com.github.User:Repo:Tag'
}
```
License
--------


    Copyright 2017 Mert Şimşek.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.




