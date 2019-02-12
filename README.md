# ValueCounter
[![](https://jitpack.io/v/Mohammed-Alaa/ValueCounter.svg)](https://jitpack.io/#Mohammed-Alaa/GifLoading)
[![License](https://img.shields.io/badge/license-Apache%202-green.svg)](https://www.apache.org/licenses/LICENSE-2.0)  

## Usage

**For a working implementation of this project see the `app/` folder.**

### Step 1

Add this in your root build.gradle at the end of repositories
```groovy
allprojects {
		repositories {
			maven { url 'https://jitpack.io' }
		}
     
}
```

### Step 2

Include the library as a local library project or add the dependency in your build.gradle.

```groovy
dependencies {
    implementation 'com.github.Mohammed-Alaa:ValueCounter:1.0.0'
}
```	

### Step 3

Add the following xml to your layout file.

```xml
<com.mohammedalaa.valuecounterlib.ValueCounterView
        app:valueColor="@color/black"
        app:defaultValue="5"
        app:addButton="@drawable/ic_add_24dp"
        app:subButton="@drawable/ic_sub_24dp"
        app:stepValue="1"
        app:minValue="1"
        app:maxValue="10"
        app:labelColor="@color/colorPrimary"
        app:labelText="EGP"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        android:id="@+id/valueCounter"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content">
    </com.mohammedalaa.valuecounterlib.ValueCounterView>
```

### Step 4

Reference the View in Java code.

```java
       ValueCounter valueCounter= (ValueCounter) findViewById(R.id.valueCounter);
```
get Value 
```java
       valueCounter.getValue();
```

  ![](/pics/demo_capture.gif =250x250)
  
  
 ## License

    Copyright 2018 Mohammmed Alaa
	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.
  
