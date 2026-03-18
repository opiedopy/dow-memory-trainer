# dow-memory-trainer
A collaboration between original code I wrote and Gemini Canvas app creator.
play it here ------- 🚀 **[Play the DOW Memory Trainer Live Here!](https://opiedopy.github.io/dow-memory-trainer/)**

Master the "Day of Week" Calendar Calculation

A high-performance, responsive web application designed to help users master the mental math of calculating the day of the week for any Gregorian date (1753–2799).

🚀 The Story

This project was built collaboratively using Gemini Canvas. In just one session, we transformed a logical Python-based algorithm into a polished, mobile-friendly interactive trainer.

🧠 The Logic (The "Jackie Dander" Method)

The trainer uses a streamlined Gregorian calculation engine. It breaks down any date into six key variables ($N1$ through $N6$):

N1: Month Reference Value (adjusted for leap years)

N2: The Day of the month

N3: Century Constant

N4: Year quotient (Last 2 digits / 12)

N5: Year remainder (Last 2 digits % 12)

N6: Remainder quotient (N5 / 4)

Final Calculation: 

$$(N1 + N2 + N3 + N4 + N5 + N6) \mod 7$$

The result (0-6) corresponds to Sunday through Saturday.

🛠️ Features

Random Test Mode: Practice your speed with randomly generated dates.

Manual Mode: Input any specific date to see the step-by-step math breakdown.

Live Stats: Tracks your accuracy, average speed, and personal best time.

Responsive UI: Built with Tailwind CSS for a premium look on both desktop and mobile.

💻 How to Run     🚀 **[Play the DOW Memory Trainer Live Here!](https://opiedopy.github.io/dow-memory-trainer/)**
or
Download index.html.

Open it in any modern web browser.

No installation or hosting required (it runs entirely client-side).

Created by Jackie Dander | Visit fuzzywidget.com
