
## SquaresLoadingView
> A SquaresLoadingView based on android.View, nicely rotation、easy to use.

[![API](https://img.shields.io/badge/API-19%2B-brightgreen.svg)](https://android-arsenal.com/api?level=19) 
[![License](https://img.shields.io/badge/license-Apache%202-green.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Download](https://img.shields.io/badge/Download-1.0.0-brightgreen.svg) ](https://github.com/fairytale110/SquaresLoadingView/archive/1.0.0.zip)

### Preview

![preview.gif](https://upload-images.jianshu.io/upload_images/1781452-f256a5f5da4f9026.gif?imageMogr2/auto-orient/strip)

### Features

Supported functions：

- [x] Optionally configure the colors of each square
- [x] Manually stop and start the animation
- [x] Configurable anim's speed

- [x] Support the padding settings


Support will be forthcoming:

- [ ] Manual rotation

- [ ] Refresh header view support

- [ ] Etc 

### How to 

To get a Git project into your build:

Step 1. Add the JitPack repository to your build file
Add it in your root build.gradle at the end of repositories:
```
  allprojects {
     repositories {
       ...
       maven { url 'https://jitpack.io' }
     }
  }
```
Step 2. Add the dependency
```
 dependencies {
     implementation 'com.github.fairytale110:SquaresLoadingView:1.0.0'
 }
```

### Usage

```java
  <tech.nicesky.bezierseekbar.BezierSeekBar
        android:id="@+id/bsBar_test"
        app:bsBar_color_ball="@android:color/white"
        app:bsBar_color_bg_selected="@android:color/white"
        app:bsBar_color_line="@android:color/white"
        app:bsBar_color_value="@android:color/white"
        app:bsBar_color_value_selected="#ef5350"
        app:bsBar_value_min="30"
        app:bsBar_value_max="120"
        app:bsBar_value_selected="65"
        app:bsBar_unit="kg"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        />
```
or
```java

   private void createBsbar() {
        fram.setBackgroundColor(Color.WHITE);
        
        BezierSeekBar seekBar = new BezierSeekBar(this);
        seekBar.setColorBall(Color.BLACK);
        seekBar.setColorLine(Color.BLACK);
        seekBar.setColorValueSelected(Color.WHITE);
        seekBar.setColorValue(Color.BLACK);
        seekBar.setColorBgSelected(Color.BLACK);
        seekBar.setValueMax(150);
        seekBar.setValueMin(20);
        seekBar.setValueSelected(60);
        seekBar.setUnit("mm");
        seekBar.setLayoutParams(new ViewGroup.LayoutParams(ViewGroup.LayoutParams.MATCH_PARENT,     ViewGroup.LayoutParams.WRAP_CONTENT));
        seekBar.setSelectedListener(new OnSelectedListener() {
            @Override
            public void onSelected(int value) {
                checkLength(value);
            }
        });
        fram.addView(seekBar);
        //checkLength(seekBar.getValueSelected());
    }
```

### Participate in the contribution
fairytale110@foxmail.com


### Author
fairytale110@foxmail.com
> 简书: http://jianshu.com/u/d95b27ffdd3c

> 掘金: https://juejin.im/user/596d91ee6fb9a06bb874a800

> CSDN: https://blog.csdn.net/LJYBQ

> MY WEB: https://nicesky.tech


## LICENSE

```
  Copyright 2018 fairytale110

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
```