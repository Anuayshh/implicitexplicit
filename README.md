# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.

## DATE : 23/08/2023

## AIM:
To create a navigate button using Implicit Intent to display the google page using Android Studio.

## EQUIPMENTS REQUIRED:
Latest Version Android Studio.

## ALGORITHM:

## Step 1: 
Open Android Studio and then click on File -> New -> New project.

## Step 2: 
Then type the Application name as HelloWorld and click Next.

## Step 3: 
Then select the Minimum SDK as shown below and click Next. 

## Step 4: 
Then select the Empty Activity and click Next. Finally click Finish. 

## Step 5: 
Design layout in activity_main.xml Step 6: Display message give in MainActivity file. Step 7: Save and run the application

## PROGRAM:
```
Program to print the text “Implicitintent”.
Developed by:V R Anu Ayshwarya
Registeration Number :212221040016
```

## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 tools:context=".MainActivity">
 <Button
 android:id="@+id/button"
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:layout_marginEnd="48dp"
 android:text="NAVIGATE"
 app:layout_constraintBottom_toBottomOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintTop_toTopOf="parent"
 app:layout_constraintVertical_bias="0.219" />
 <EditText
 android:id="@+id/editTextTextPersonName"
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:layout_marginStart="32dp"
 android:ems="10"
 android:inputType="textPersonName"
 app:layout_constraintBottom_toBottomOf="parent"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toTopOf="parent"
 app:layout_constraintVertical_bias="0.218" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.ex3;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.net.Uri;
import android.widget.Button;
import android.widget.EditText;
import android.os.Bundle;
public class MainActivity extends AppCompatActivity {
 Button button;
 EditText editText;
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
 button = findViewById(R.id.button);
 editText = findViewById(R.id.editTextTextPersonName);
 button.setOnClickListener(view -> {
 String url=editText.getText().toString();
 Intent intent=new Intent(Intent.ACTION_VIEW, Uri.parse(url));
 startActivity(intent);
 });
 } }
```
## Output:

![image](https://github.com/Anuayshh/implicitexplicit/assets/127651217/1682f4f4-8de3-4ca3-9308-aea5121628c6)
![image](https://github.com/Anuayshh/implicitexplicit/assets/127651217/391483a3-0fc2-415a-93c6-ba3f99a7e6b0)

![Uploading image.png…]()







## RESULT:
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.



