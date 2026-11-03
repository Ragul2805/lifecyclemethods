# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


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
Developed by: Ragul D
Registeration Number : 212225230221
*/
```
## MainActivity.Java
```
package com.example.test;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(getApplicationContext(),"Create Enabled",Toast.LENGTH_LONG);
        t.show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast t=Toast.makeText(getApplicationContext(),"Restart Enabled",Toast.LENGTH_LONG);
        t.show();
    }
    @Override
    protected void onStart() {
        super.onStart();
        Toast t=Toast.makeText(getApplicationContext(),"Start Enabled",Toast.LENGTH_LONG);
        t.show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Toast t=Toast.makeText(getApplicationContext(),"Resume Enabled",Toast.LENGTH_LONG);
        t.show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Toast t=Toast.makeText(getApplicationContext(),"Pause Enabled",Toast.LENGTH_LONG);
        t.show();
    }

    @Override
    protected void onStop() {
        super.onStop();
        Toast t=Toast.makeText(getApplicationContext(),"Stop Enabled",Toast.LENGTH_LONG);
        t.show();
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Toast t=Toast.makeText(getApplicationContext(),"Destroy Enabled",Toast.LENGTH_LONG);
        t.show();
    }
}
```
## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Life Cycle Activity!"
        android:textSize="24sp"
        android:background="#FF0"
        app:layout_constraintBottom_toTopOf="@+id/textView"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.295" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="320dp"
        android:text="Welcome to Android Studio"
        android:textSize="23sp"
        android:textColor="#FF00"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT
<img width="1366" height="720" alt="mui 1" src="https://github.com/user-attachments/assets/687cc85b-773c-49d8-9206-d982fbb5cf92" />

**OnCreate**
<img width="1366" height="720" alt="mui 2" src="https://github.com/user-attachments/assets/f9b7f209-9f70-4afd-9a78-36810d5ad73b" />


**OnStart**
<img width="1366" height="720" alt="mui 3" src="https://github.com/user-attachments/assets/4026f20c-176c-465b-b7df-b9fdf0de9741" />


**OnRestart**
<img width="1366" height="720" alt="muib 5" src="https://github.com/user-attachments/assets/183b6519-e43e-4642-8849-ab8195becbe2" />


**OnResume**
<img width="1366" height="720" alt="muib 4" src="https://github.com/user-attachments/assets/ad848c92-7689-461a-9c9f-8075d29c61fe" />


**OnPause**
<img width="1366" height="720" alt="muib 6" src="https://github.com/user-attachments/assets/e192b7ef-3f60-44f3-a077-a7389120ec3f" />









## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
