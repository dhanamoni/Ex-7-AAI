<H3>ENTER YOUR NAME : MONIKA D</H3>
<H3>ENTER YOUR REGISTER NO: 212223240096</H3>
<H3>EX. NO.7</H3>
<H3>DATE:14.05.2025</H3>
<H1 ALIGN =CENTER>Implementation of Text  Summarization</H1>
<H3>Aim: to perform automatic text summarization using Natural Language Processing (NLP) techniques. </H3> 
 <BR>
<h3>Algorithm:</h3>
Step 1 Import necessary libraries for natural language processing tasks.<BR>
Step 2: Download NLTK resources, including the punkt tokenizer and stopwords.<BR>
Step 3: Define Text Preprocessing Function to tokenize, remove stopwords, and perform stemming.<BR>
Step 4: Define the Text Summarization Function using a simple frequency-based approach.<br>
    - Calculate the frequency of each word in the preprocessed text.<br>
    - Calculate a score for each sentence based on the sum of word frequencies.<br>
    - Select the top N sentences with the highest scores to form the summary.<br>
Step 5: Construct the main program to read the paragraph  and perform text summarization<br>
      - Generate and print the original text.<br>
      - Generate and print the text summary using the  Text Summarization function<br>
      
## Program:
~~~
pip install SpeechRecognition
pip install pyaudio

import speech_recognition as sr
r = sr.Recognizer()

duration = 15
print("Say something:")

with sr.Microphone() as source :
    audio_data = r.listen(source,timeout = duration)

try:
    text = r.recognize_google(audio_data)
    print("You said:", text)
except sr.UnknownValueError:
    print("Sorry, could not understand audio")
except sr.RequestError as e:
    print(f'Error with the request to Google Speech Recognition service: {e}')
except Exception as e:
    print(f'Error: {e}')
~~~

## Output:

![image](https://github.com/user-attachments/assets/b13cb01e-b90d-4bea-9975-146adacbf629)


## Result:
Thus ,the program to perform the Text summarization is executed sucessfully.


