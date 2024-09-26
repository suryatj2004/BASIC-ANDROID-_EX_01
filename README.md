# Ex.No:1 Implementation of a Hello world Activity using all lifecycles methods using Android Studio.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)
## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to implement a Hello world Activity using all lifecycles methods using Android Studio .
Developed by: KAVIYARASU.K
RegisterNumber: 212222040075
*/
```
# MainActivity.java:
```
mainactivity.java
package com.example.bala;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart()
    {

        super.onRestart();
        Toast toast =Toast.makeText(getApplicationContext(),"onReStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart()
    {

        super.onStart();
        Toast toast =Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume()
    {

        super.onResume();
        Toast toast =Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause()
    {

        super.onPause();
        Toast toast =Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop()
    {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy()
    {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }

}
```
# activitymain.xml:
```
androidmanifest.xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.Bala"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## OUTPUT:

## Onstart:
![lc1](https://github.com/Samuelmariappan/lifecyclemethods/assets/119393030/8f206bbd-26f0-4593-b625-215084dead67)

## Onrestart:
![lc2](https://github.com/Samuelmariappan/lifecyclemethods/assets/119393030/9b7a56a3-2cb0-47dc-a9e8-669c51e9d804)

## Onresume:
![lc3](https://github.com/Samuelmariappan/lifecyclemethods/assets/119393030/3e836d5f-7cfb-4d1c-898f-de8f8e84fc7c)

## Oncreate:
![lc4](https://github.com/Samuelmariappan/lifecyclemethods/assets/119393030/e756a4f7-e1ad-4480-b97c-1c5303e7b20d)

## Onpause:
![lc5](https://github.com/Samuelmariappan/lifecyclemethods/assets/119393030/726d829f-7e8a-4619-aee9-43355a4f19bb)


## RESULT
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
