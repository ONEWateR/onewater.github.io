---
layout: post
title: 改变ToolBar的Title颜色
---
## 小问题
如何改变Toolbar的title的颜色呢？

## 方法

`Style.xml`

    <resources>

        <style name="AppTheme" parent="Theme.AppCompat.Light">
            <item name="colorPrimary">@color/primary</item>
            <item name="colorPrimaryDark">@color/primary_dark</item>
            <item name="colorAccent">@color/accent</item>
        </style>

        <style name="AppTheme.ToolbarActivity" parent="AppTheme">
            <item name="toolbarStyle">@style/Toolbar</item>
        </style>

        <style name="Toolbar" parent="Widget.AppCompat.Toolbar">
            <item name="android:background">?attr/colorPrimary</item>
            <item name="android:minHeight">?attr/actionBarSize</item>
            <item name="titleTextAppearance">@style/TitleStyle</item>
        </style>

        <style name="TitleStyle" parent="TextAppearance.Widget.AppCompat.Toolbar.Title">
            <item name="android:textColor">@android:color/white</item>
        </style>

    </resources>
    

好吧，有点水了。