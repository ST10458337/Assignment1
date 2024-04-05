package com.example.assignment1

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.widget.Button
import android.widget.EditText
import android.widget.TextView

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        /* Declaring variables */
        val ageInput = findViewById<EditText>(R.id.edtAgeInput)
        val historyText = findViewById<TextView>(R.id.txtDisplay)
        val btnHistory = findViewById<Button>(R.id.btnGenerate)
        val btnClear = findViewById<Button>(R.id.btnClear)

        /* Process for the Generate History button */
        btnHistory.setOnClickListener {
            val edtInput = ageInput.text.toString()
            val age = edtInput.toIntOrNull()
            var ageHistory = ""

            /* If else statements for checking the age the user inputs */
            if(age==20)
            {
                ageHistory = "Pocahontas died at 20. She is known for helping English colonists in Virginia specifically a Captain John Smith."
                /* (The Famous People,no date) */

            }
            else if (age==21)
            {
                ageHistory = "Sophie Scholl died at 21. An anti-Nazi activist who was executed by guillotine. Many films based on her have been produced."
                /* (The Famous People,no date) */
            }
            else if (age==22)
            {
                ageHistory = "Aaliyah died at 22. A prestigious singer who's first album sold 3 million copies. She died in an airplane crash."
                /* (The Famous People,no date) */
            }
            else if (age==23)
            {
                ageHistory = "Gavrilo Princip died at 23. In an attempt to free Bosnia and Herzegovina he assassinated an Austrian archduke, a action that would soon lead to World War 1."
                /* (The Famous People,no date) */
            }
            else if (age==24)
            {
                ageHistory = "The Notorious B.I.G. died at 24. A rapper who is considered to be one of the greatest in hip-hop, he was killed in a drive-by shooting."
                /* (The Famous People,no date) */
            }
            else if (age==25)
            {
                ageHistory = "Jules Bianchi died at 25. A champion of the Formula 3 Euro Series, he got in a collision which put him in a coma for 8 months before eventually dying."
                /* (The Famous People,no date) */
            }
            else if (age==26)
            {
                ageHistory = "Otis Redding died at 26. An iconic singer who is regarded as The King of Soul"
                /* (The Famous People,no date) */
            }
            else if (age==27)
            {
                ageHistory = "Jimi Hendrix died at 27. One of the most iconic and innovative Rock and Roll figures."
                /* (The Famous People,no date) */
            }
            else if (age==28)
            {
                ageHistory = "Heath Ledger died at 28. An amazing actor known mostly for his performance on The Dark Knight as The Joker."
                /* (The Famous People,no date) */
            }
            else if (age==29)
            {
                ageHistory = "Jesus Christ died at 29. The Son Of God who's preaching eventually began Christianity. He was crucified by the Roman government but later rose from the dead."
                /* (The Famous People,no date) */
            }
            else if (age==30)
            {
                ageHistory = "Nero died at 30. The tyrannical fifth emperor of Rome, he is responsible for the death of his mother, the Great fire of Rome, and the deaths of many Christians"
                /* (The Famous People,no date) */
            }
            else /* Error handling for an out of range input by the user */
            {
                ageHistory = "The age is out of ramge. Please enter a age from 20 - 30"
            }
            if (ageHistory == null)
            {
                historyText.text = "Please enter a whole number (e.g. 20, 21, 22). Texts or decimals are invalid."
            }

            historyText.text = ageHistory
        }
        btnClear.setOnClickListener {
            ageInput.text.clear()
            historyText.text = ""
        }
        /* REFERENCE LIST */
        /*The Famous People. (no date). Famous people who died at 20, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-20.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 21, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-21.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 22, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-22.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 23, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-23.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 24, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-24.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 25, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-25.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 26, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-26.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 27, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-27.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 28, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-28.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 29, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-29.php [Accessed 3 April 2024]. */
        /*The Famous People. (no date). Famous people who died at 30, (no date).[Online]. Available at:https://www.thefamouspeople.com/died-at-30.php [Accessed 3 April 2024]. */
    }
}
