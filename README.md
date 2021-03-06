# SpeedView
Dynamic Speedometer UI for Android :zap: , you can change the color of everything.

`minSdkVersion=11`

Library Size ~ 6 Kb.

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-SpeedView-green.svg?style=true)](https://android-arsenal.com/details/1/4169)

<img src="/images/SpeedView.gif" width="96%" /><br/>
<img src="/images/SpeedView1.png" width="24%" />
<img src="/images/SpeedView2.png" width="24%" />
<img src="/images/SpeedView3.png" width="24%" />
<img src="/images/SpeedView4.png" width="24%" />

# dependencies 

**add this line to** `build.gradle`

```gradle

dependencies {
	    compile 'com.github.anastr:speedviewlib:1.0.0'
}

```

# Usage

**add SpeedView to your layout**

```xml

<com.github.anastr.speedviewlib.SpeedView
        android:id="@+id/speedView"
        android:layout_width="250dp"
        android:layout_height="wrap_content" />

```

change the **speed** from your code : 

```java

SpeedView speedView = (SpeedView) findViewById(R.id.speedView);

// change speed to 50 Km/h
speedView.speedTo(50);

// you can change max speed by this line (default : 100)
speedView.setMaxSpeed(220);

/** 
  * see also:
  * speedView.setWithTremble(false);
  * speedView.setIndicatorColor(Color.BLUE);
  * speedView.setHighSpeedColor(Color.RED);
  * .....
  */

```

and also you can change everything in XML, see this Attributes : 

```xml

app:maxSpeed="220" <!-- def : 100 -->
app:withTremble="false" <!-- def : true -->
app:speedometerWidth="35dp" <!-- def : 30dp -->
app:indicatorColor="#2b38e6" <!-- def : BLACK -->
app:centerCircleColor="#b2f941ff" <!-- def : GRAY -->
app:lowSpeedColor="#58ed21" <!-- def : GREEN -->
app:mediumSpeedColor="#edd029" <!-- def : YELLOW -->
app:highSpeedColor="#ec2f33" <!-- def : RED -->
app:markColor="#99000000" <!-- def : DKGRAY -->
app:textColor="#e23900" <!-- def : BLACK -->

```

<img src="/images/SpeedView.png" width="100%" /><br/>


# LICENSE
```

Copyright 2016 Anas ALtair

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
