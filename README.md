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
Program to print the text “Welcome to Android Studio”.
Developed by: Monisha D
Registeration Number : 212225240090
*/
```

## MainActivity.java
```
package com.example.text;

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
        Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG).show();
    }
    protected void onStart(){
        super.onStart();
        Toast.makeText(getApplicationContext(),"onStart Called", Toast.LENGTH_LONG).show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast.makeText(getApplicationContext(),"onRestart Called", Toast.LENGTH_LONG).show();
    }
    protected void onPause(){
        super.onPause();
        Toast.makeText(getApplicationContext(),"onPause Called", Toast.LENGTH_LONG).show();
    }
    protected void onResume(){
        super.onResume();
        Toast.makeText(getApplicationContext(),"onResume Called", Toast.LENGTH_LONG).show();
    }
    protected void onStop(){
        super.onStop();
        Toast.makeText(getApplicationContext(),"onStop Called", Toast.LENGTH_LONG).show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast.makeText(getApplicationContext(),"onDestroy", Toast.LENGTH_LONG).show();
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
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Welcome to Android studio"
        android:textSize="18sp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT
<img width="1919" height="1020" alt="Screenshot 2026-10-30 082913" src="https://github.com/user-attachments/assets/f0df31d6-523e-488d-89db-b8a759c9019e" />

<img width="1919" height="1021" alt="Screenshot 2026-10-30 082950" src="https://github.com/user-attachments/assets/09a12367-3b96-46f6-bfc1-2908a399c03d" />

<img width="1918" height="1020" alt="Screenshot 2026-10-30 083037" src="https://github.com/user-attachments/assets/892c5725-161c-4039-859e-1a9a3a0fd072" />

<img width="1919" height="1024" alt="Screenshot 2026-10-30 083154" src="https://github.com/user-attachments/assets/014cd33f-c52f-4157-af12-f38fa238a0cd" />

<img width="1919" height="1022" alt="Screenshot 2026-10-30 083104" src="https://github.com/user-attachments/assets/1e602dde-f947-454d-91d7-3c4dd50ca52b" />



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
