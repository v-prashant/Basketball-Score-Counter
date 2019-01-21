
## code counter java code


package com.example.android.courtcounter;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    int scoreteamA=0;
    int scoreteamB=0;


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


    }

    public void threeforteamA(View v)
    {
        scoreteamA=scoreteamA+3;
        displayforteamA(scoreteamA);
    }


    public void twoforteamA(View v)
    {
        scoreteamA=scoreteamA+2;
        displayforteamA(scoreteamA);
    }


    public void oneforteamA(View v)
    {
        scoreteamA=scoreteamA+1;
        displayforteamA(scoreteamA);
    }



    public void threeforteamB(View v)
    {
        scoreteamB=scoreteamB+3;
        displayforteamB(scoreteamB);
    }


    public void twoforteamB(View v)
    {
        scoreteamB=scoreteamB+2;
        displayforteamB(scoreteamB);
    }


    public void oneforteamB(View v)
    {
        scoreteamB=scoreteamB+1;
        displayforteamB(scoreteamB);
    }

    public void resetscore(View v)
    {
        scoreteamA=0;
        scoreteamB=0;
        displayforteamA(scoreteamA);
        displayforteamB(scoreteamB);
    }

    public void displayforteamA(int score)
    {
        TextView scoreView = (TextView) findViewById(R.id.team_a_score);
        scoreView.setText(String.valueOf(score));
    }

    public void displayforteamB(int score)
    {
        TextView scoreView = (TextView) findViewById(R.id.team_b_score);
        scoreView.setText(String.valueOf(score));
    }
}
