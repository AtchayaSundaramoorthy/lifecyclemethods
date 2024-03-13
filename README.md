# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

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
Program to print the text “Hello World”.
Developed by:
Registeration Number :
*/
```
##MainActivity.java
```Java
package com.example.myproj1;

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
    protected void onStart()
    {
        // It will show a message on the screen
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart()
    {
        // It will show a message on the screen
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume()
    {
        // It will show a message on the screen
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause()
    {
        // It will show a message on the screen
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop()
    {
        // It will show a message on the screen
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy()
    {
        // It will show a message on the screen
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```
##Activity_main.xml
```Java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:rotation="0"
    android:visibility="visible"
    tools:context=".MainActivity"
    tools:visibility="visible">

    <TextView
        android:id="@+id/textView"
        android:layout_width="114dp"
        android:layout_height="83dp"
        android:text="Hello World"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.499" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
##AndroidManifest.xml
```Java
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
        android:theme="@style/Theme.Myproj1"
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

## OUTPUT
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/3e491367-9715-4213-b894-f4a01107837d)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/8252470d-574c-4060-94df-4717065d5952)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/d6c6591c-b329-48e6-9b79-476da2e7405f)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/77d5299f-ebb5-4dda-b9f0-92d5caf0b289)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/fac44a03-2911-4477-8757-6516dec64afe)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/c16f2c1b-e78a-4875-b962-cfe51efd03c7)
![image](https://github.com/AtchayaSundaramoorthy/lifecyclemethods/assets/119393516/eadbfd7d-9687-4011-95ee-cceda132efd6)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
