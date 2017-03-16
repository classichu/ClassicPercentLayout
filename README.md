# ClassicPercentLayout

Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
Step 2. Add the dependency

	dependencies {
	        compile 'com.github.classichu:ClassicPercentLayout:x.x.x'
	}



 



xml


	<?xml version="1.0" encoding="utf-8"?>
	<android.support.percent.PercentFrameLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.classichu.classicpercentlayout.MainActivity">

    <android.support.percent.PercentRelativeLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        >

        <TextView
            android:id="@+id/id_left"
            android:layout_width="0dp"
            android:layout_height="0dp"
            android:text="LEFT"
            android:background="@color/colorAccent"
            app:layout_heightPercent="20%"
            app:layout_widthPercent="30%"
            />

        <TextView
            android:layout_width="0dp"
            android:layout_height="0dp"
            android:text="RIGHT"
            android:layout_toRightOf="@id/id_left"
            android:background="@color/colorPrimary"
            app:layout_heightPercent="50%"
            app:layout_widthPercent="30%" />


    </android.support.percent.PercentRelativeLayout>


 	<com.classichu.percentlayout.PercentLinearLayout
     android:orientation="horizontal"
     android:layout_width="wrap_content"
     android:layout_gravity="bottom"
     android:layout_height="wrap_content"
     >
     <TextView
         android:layout_width="0dp"
         android:layout_height="0dp"
         android:text="left"
         android:background="#b28d0a"
         app:layout_heightPercent="40%"
         app:layout_widthPercent="70%"
         />

     <TextView
         android:layout_width="0dp"
         android:layout_height="0dp"
         android:text="right"
         android:background="#2a7c2c"
         app:layout_heightPercent="10%"
         app:layout_widthPercent="30%" />


 		</com.classichu.percentlayout.PercentLinearLayout>

	</android.support.percent.PercentFrameLayout>
