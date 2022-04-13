
# Rapport

I denna uppgift gjordes en layout till MainActivity som innehöll en ImageView, en TextView, två EditText och en ButtonView. Dessa var upplagda som en login-skärm.
För att fylla i all text på sidan skapades nya strings i strings.xml, istället för att hardcodea in texten i layouten.
Sen skapades även en clickhandler till knappen och en Log.d användes för att se om knappen blivit klickad i logcat.

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

Exempel på hur en av de skapade EditView såg ut:
```
<EditText
    android:id="@+id/login_input_username"
    android:layout_width="250dp"
    android:layout_height="wrap_content"
    android:layout_marginTop="16dp"
    android:autofillHints="username"
    android:hint="@string/login_username_hint"
    android:inputType="text"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/login_info" />
```

Skapandet av onclickhandler:
```
login_button = findViewById(R.id.login_button);
login_button.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        Log.d("===", "The login button has been pressed!");
    }
});
```

Det finns en bild ovanför login-rutan, men av någon anledning syns den inte i emulatorn.
![](screenshot.png)
