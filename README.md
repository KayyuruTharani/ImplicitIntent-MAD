# Ex.No:3a Develop program to create a text field and a button “Navigate”. When you enter “www.gmail.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the gmail page using Android Studio.

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
Program to print the text “Implicitintent”.
Developed by: Kayyuru Tharani
Registeration Number : 212221040080
*/


package com.example.implicitintent;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        EditText editText;
        Button button;

        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        button = findViewById(R.id.button);

        editText = (EditText) findViewById(R.id.editTextText2);


        button.setOnClickListener(new View.OnClickListener() {

            @Override

            public void onClick(View view) {

                String url=editText.getText().toString();

                Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse(url));

                startActivity(intent);

            }

        });




    }
}
```

## OUTPUT

![Screenshot (92)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/49e24697-42c9-4020-bcd5-55c1c1f18879)

![Screenshot (93)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/42f48751-384b-46c1-a0aa-da0b3200c23d)

![Screenshot (94)](https://github.com/KayyuruTharani/ImplicitIntent-MAD/assets/142209319/9ce01b24-97c8-4cad-958f-5788d99477bf)








## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the gmail page using Android Studio is developed and executed successfully.


