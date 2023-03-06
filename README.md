# FrancAIs
Demo of using ChatGPT API for language learning

March 6, 2023

Here is a demo of the pedagogical potential of ChatGPT.  I wrote this web app in one day, with no pre-existing knowledge whatsoever of Flask or AJAX.  I used GPT to assist in writing the code and site, and of course GPT3.5 is powering the back-end of this app.

CONCEPT: AI-based language learning.  In this case, French for an intermediate learning.  It would be trivial to adjust this for different languages, both user languages and target being learned.  It is also trivial to adjust the level of difficulty, which could also be programmed in.

WHAT THE APP DOES: It takes the top story on Le Monde, grabs three paragraphs of text, and prepares questions about the vocabulary, grammar and idioms.  The user inputs are converted into prompts which are better suited for training students and pointing out minor flaws and why they might have occurred.  Using this app every day would cost roughly USD 15 cents per month.

EXTENSIONS: This is just a proof of concept, but of course, it can be extended to retain a database of target words, to use spaced repetition on those words and grammar concepts, to adjust for the language level of the student automatically, and so on.  The basic point is that with no knowledge of linguistics education, web app programming, or computer science, you can produce an app like this in one day. Knowing what I now know, I could do it a second time in a couple hours.

HOW TO USE: The app is python using flask.  You need Python as well as an OpenAI key, which you can get for free. Put you key in a file called APIkey.txt in your working directory, app.py in the same directory, and index.html in a Templates subdirectory.   One you have python 3.7+ installed, the easiest way to run it is to open a python instance.
In Windows, open a command prompt with cmd
cd to the folder you want to run this program
type py -m venv env to open a virtual environment
type env\Scripts\activate.bat 
type set FLASK_APP=app so Flask knows to run the program "app"
pip install each of the libraries in the code
type flask run
open http://localhost:5000/ in your web browser

Now you are good to go!  Note that the code is somewhat stochastic, so if you reload you will get different questions. 
