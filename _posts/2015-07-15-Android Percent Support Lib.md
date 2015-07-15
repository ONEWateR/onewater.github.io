---
layout: post
title: Android Percent Support Lib 使用
---


## 概述
Android Percent Support Lib 是一个支持百分比布局的类库。


## 使用

```xml
dependencies {
    compile 'com.android.support:percent:22.2.0'
}
```


###支持的Layouts :

代码来自[android-percent-support-lib-sample](https://github.com/JulienGenoud/android-percent-support-lib-sample)


####PercentRelativeLayout

```xml
<android.support.percent.PercentRelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    
    <View
        android:id="@+id/top_left"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_alignParentTop="true"
        android:background="#ff44aacc"
        app:layout_heightPercent="20%"
        app:layout_widthPercent="70%" />

    <View
        android:id="@+id/top_right"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_alignParentTop="true"
        android:layout_toRightOf="@+id/top_left"
        android:background="#ffe40000"
        app:layout_heightPercent="20%"
        app:layout_widthPercent="30%" />


    <View
        android:id="@+id/bottom"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_below="@+id/top_left"
        android:background="#ff00ff22"
        app:layout_heightPercent="80%" />
</android.support.percent.PercentRelativeLayout>
```

####PercentLinearLayout
```xml
<com.juliengenoud.percentsamples.PercentLinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">
     <View
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:background="#ff44aacc"
        app:layout_heightPercent="10%"
        app:layout_widthPercent="60%"/>

    <View
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:background="#ff4400cc"
        app:layout_heightPercent="10%"
        app:layout_widthPercent="70%"/>
</com.juliengenoud.percentsamples.PercentLinearLayout>
```

####PercentFrameLayout
```xml
<android.support.percent.PercentFrameLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
        <!-- ... XML CODE -->
</android.support.percent.PercentFrameLayout>
```



###Stylable :

- heightPercent
- widthPercent
- marginBottomPercent
- marginEndPercent
- marginLeftPercent
- marginPercent
- marginRightPercent 
- marginStartPercent
- marginTopPercent
