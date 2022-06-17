package com.example.calculadora_tentativa_2;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private EditText txtNr1;
    private EditText txtNr2;
    private TextView tvResultado;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        txtNr1 = findViewById(R.id.txtNr1);
        txtNr2 = findViewById(R.id.txtNr2);
        tvResultado = findViewById(R.id.tvResultado);


    }

    public void somar(View view) {

        double valor1 = Integer.parseInt(txtNr1.getText().toString());
        double valor2 = Integer.parseInt(txtNr2.getText().toString());

        tvResultado.setText(String.valueOf(valor1 + valor2));

    }

    public void subtrair(View view) {

        double valor1 = Integer.parseInt(txtNr1.getText().toString());
        double valor2 = Integer.parseInt(txtNr2.getText().toString());

        tvResultado.setText(String.valueOf(valor1 - valor2));
    }

    public void multiplicar(View view) {

        double valor1 = Integer.parseInt(txtNr1.getText().toString());
        double valor2 = Integer.parseInt(txtNr2.getText().toString());

        tvResultado.setText(String.valueOf(valor1 * valor2));
    }

    public void dividir(View view) {

        double valor1 = Integer.parseInt(txtNr1.getText().toString());
        double valor2 = Integer.parseInt(txtNr2.getText().toString());

        tvResultado.setText(String.valueOf(valor1 / valor2));
    }
