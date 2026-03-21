# dow-memory-trainer
A collaboration between original code I wrote and Gemini Canvas app creator.
play it here ------- 🚀 **[Play the DOW Memory Trainer Live Here!](https://opiedopy.github.io/dow-memory-trainer/)**
On edit: After three days, I though I was finished, but I sent the html code to Claude for review and Claude found 11 things to improve upon. 
So, thanks to both Gemini and Claude.  I asked Claude if it wanted to start from scratch and it said, no way, let's build upon what you have alrady done. Impressive from both Ai's.
But: I have to say that is is best to include the working html code for them to edit because if you don't there may be an hallucination or 
error about what previous code to use.  I learned that the hard way and it cost me two days of work.

Master the "Day of Week" Calendar Calculation

A high-performance, responsive web application designed to help users master the mental math of calculating the day of the week for any Gregorian date (1753–2799).

🚀 The Story

This project was built collaboratively using Gemini Canvas. In just one session, we transformed my own logical Python-based algorithm into a polished, mobile-friendly interactive trainer.

🧠 The Logic (The "Jackie Dander" Method)

The trainer uses a streamlined Gregorian calculation engine. It breaks down any date into six key variables (N1 through N6):

N1: Month Reference Value (adjusted for leap years)

N2: The Day of the month

N3: Century Constant

N4: Year quotient (Last 2 digits / 12)

N5: Year remainder (Last 2 digits % 12)

N6: Remainder quotient (N5 / 4)

Final Calculation: 

(N1 + N2 + N3 + N4 + N5 + N6) \mod 7

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
=============================
Document follows, repeating some of the above:
"""Day of Week (DOW) Calculation 
(Years 1753 to 9999) (restriction is due to different calendars used prior to 1753 and the possible Revised Julian Calendar used after February 29, 2800)
CREATED BY JACKIE DANDER OF FUZZYWIDGET.COM, TODAY IS Dec 5, 2025 
Copyright. May be used or copied with attribution. 
For use by mental math or converting to micro python code for input: Month, day, year.
Note: The python modulo operator is "%".  Example: 76%12 = 4 

For example: What day of the week is February 29, 2052?
1. Month = -1
2. Day = 29
3. “20” = century (CC) = 2
4. “52” = year (YY/12) = 4
5. “52” = year (YY%12) = 4
6. “52” = year (integer of #5 answer /4) = 1

Answer is (sum above or -1 + 29 + 2 + 4 + 4 + 1 = 39, and 39%7 = 4, so DOW = Thursday.
""" 

1. Month values   =  	 4,  0,  0,  3,  5,  1,  3,  6,  2,  4,  0,  2 
But, if leap year:  = 	 3, -1,  0,  3,  5,  1,  3,  6,  2,  4,  0,  2 

2. Day = day 

3. century calculation values, (Note: 400 year repeating  
centurylist = [2, 0, 5, 3] beginning with 1600.) 
Example: 
2000 is 2 
2100 is 0 
2200 is 5 
2300 is 3 
2400 is 2.  Etc etc 

4. Integer of YY/12 

5. Modulo = YY%12 

6. Integer of (answer above)/4 
_______________________ 

Add 1 thru 6 = 

Answer is (after modulo 7) = 

0 1 2 3 4 5 6 

Sun Mon Tue Wed Thu Fri Sat


