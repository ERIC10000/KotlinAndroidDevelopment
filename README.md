# KotlinAndroidDevelopment
## Android Studion App Structure
### 1. Manifest
It containns configuration information about the app
### 2. Java
Contain all the kotlin files for developing android logics
### 3. Res
Contains all the resources reuired for the app
### 4. Gradle
Dependancies required for the app are configured here

## The Dashboard Project
### Step1: Drawable file 
Drawables are used to create shapes, icon in android application
In the drawable folder, create a file called custom_background.xml and paste the code below:

```
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="rectangle">

    <solid
        android:color="@color/purple_700"/>

    <corners
        android:topLeftRadius="400dp"
        android:topRightRadius="0dp"/>

</shape>
```

### Step2: Vecor Assets
With vector assets, we are able to create icons for the applications

#### Home Icon -> ic_home.xml
```
<vector android:height="50dp" android:tint="#4A148C"
    android:viewportHeight="24" android:viewportWidth="24"
    android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M10,20v-6h4v6h5v-8h3L12,3 2,12h3v8z"/>
</vector>
```
#### Chat Icon -> ic_chat.xml
```
<vector android:autoMirrored="true" android:height="50dp"
    android:tint="#4A148C" android:viewportHeight="24"
    android:viewportWidth="24" android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M20,2L4,2c-1.1,0 -1.99,0.9 -1.99,2L2,22l4,-4h14c1.1,0 2,-0.9 2,-2L22,4c0,-1.1 -0.9,-2 -2,-2zM6,9h12v2L6,11L6,9zM14,14L6,14v-2h8v2zM18,8L6,8L6,6h12v2z"/>
</vector>
```
#### Profile Icon -> ic_profile.xml
```
<vector android:height="50dp" android:tint="#4A148C"
    android:viewportHeight="24" android:viewportWidth="24"
    android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M12,12c2.21,0 4,-1.79 4,-4s-1.79,-4 -4,-4 -4,1.79 -4,4 1.79,4 4,4zM12,14c-2.67,0 -8,1.34 -8,4v2h16v-2c0,-2.66 -5.33,-4 -8,-4z"/>
</vector>

```

#### Settings Icon -> ic_settings.xml
```
<vector android:height="50dp" android:tint="#4A148C"
    android:viewportHeight="24" android:viewportWidth="24"
    android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M19.14,12.94c0.04,-0.3 0.06,-0.61 0.06,-0.94c0,-0.32 -0.02,-0.64 -0.07,-0.94l2.03,-1.58c0.18,-0.14 0.23,-0.41 0.12,-0.61l-1.92,-3.32c-0.12,-0.22 -0.37,-0.29 -0.59,-0.22l-2.39,0.96c-0.5,-0.38 -1.03,-0.7 -1.62,-0.94L14.4,2.81c-0.04,-0.24 -0.24,-0.41 -0.48,-0.41h-3.84c-0.24,0 -0.43,0.17 -0.47,0.41L9.25,5.35C8.66,5.59 8.12,5.92 7.63,6.29L5.24,5.33c-0.22,-0.08 -0.47,0 -0.59,0.22L2.74,8.87C2.62,9.08 2.66,9.34 2.86,9.48l2.03,1.58C4.84,11.36 4.8,11.69 4.8,12s0.02,0.64 0.07,0.94l-2.03,1.58c-0.18,0.14 -0.23,0.41 -0.12,0.61l1.92,3.32c0.12,0.22 0.37,0.29 0.59,0.22l2.39,-0.96c0.5,0.38 1.03,0.7 1.62,0.94l0.36,2.54c0.05,0.24 0.24,0.41 0.48,0.41h3.84c0.24,0 0.44,-0.17 0.47,-0.41l0.36,-2.54c0.59,-0.24 1.13,-0.56 1.62,-0.94l2.39,0.96c0.22,0.08 0.47,0 0.59,-0.22l1.92,-3.32c0.12,-0.22 0.07,-0.47 -0.12,-0.61L19.14,12.94zM12,15.6c-1.98,0 -3.6,-1.62 -3.6,-3.6s1.62,-3.6 3.6,-3.6s3.6,1.62 3.6,3.6S13.98,15.6 12,15.6z"/>
</vector>
```
#### Widgets Icon -> ic_widgets.xml
```
<vector android:height="50dp" android:tint="#4A148C"
    android:viewportHeight="24" android:viewportWidth="24"
    android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M13,13v8h8v-8h-8zM3,21h8v-8L3,13v8zM3,3v8h8L11,3L3,3zM16.66,1.69L11,7.34 16.66,13l5.66,-5.66 -5.66,-5.65z"/>
</vector>
```

#### Logout Icon -> ic_logout.xml
```
<vector android:autoMirrored="true" android:height="50dp"
    android:tint="#4A148C" android:viewportHeight="24"
    android:viewportWidth="24" android:width="50dp" xmlns:android="http://schemas.android.com/apk/res/android">
    <path android:fillColor="@android:color/white" android:pathData="M17,7l-1.41,1.41L18.17,11H8v2h10.17l-2.58,2.58L17,17l5,-5zM4,5h8V3H4c-1.1,0 -2,0.9 -2,2v14c0,1.1 0.9,2 2,2h8v-2H4V5z"/>
</vector>
```

## The Dashboard Layout -> proceed to Layout
Open the file activity_maim.xml, Paste the code below

```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@drawable/custom_background"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="My Dashboard"
        android:layout_margin="12dp"
        android:textColor="@color/black"
        android:textSize="30dp"
        android:textStyle="bold"/>

    <GridLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_below="@+id/textView"
        android:layout_marginTop="20dp"
        android:layout_margin="20dp"
        android:columnCount="2"
        android:rowCount="3">

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="0"
            android:layout_row="0">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_home"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Home"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="1"
            android:layout_row="0">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_chat"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Chats"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="0"
            android:layout_row="1">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_profile"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Profile"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="1"
            android:layout_row="1">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_widgets"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Widgets"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="0"
            android:layout_row="2">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_settings"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Settings"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="fill"
            android:layout_rowWeight="1"
            android:layout_columnWeight="1"
            android:background="@color/white"
            app:cardCornerRadius="8dp"
            app:cardElevation="8dp"
            app:cardUseCompatPadding="true"
            android:layout_column="1"
            android:layout_row="2">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="center_horizontal|center_vertical"
                android:gravity="center"
                android:orientation="vertical">

                <ImageView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:src="@drawable/ic_logout"/>

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Logout"
                    android:textSize="16sp"
                    android:textColor="@color/black"/>

            </LinearLayout>


        </androidx.cardview.widget.CardView>

    </GridLayout>

</RelativeLayout>
```
