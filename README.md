# Emotion-Recognition-based-Voice-of-Citizen
 
 
The scope of this study is to identify the tweets about Bangalore traffic and analyze the data and recognize the eight emotions (Joy, Anger, Fear, Sadness, Disgust, Anticipation, Trust, and Surprise) from the data. This is further used to provide a dashboard to show the tweet classification and frequencies based on emotions identified
 
![image](https://user-images.githubusercontent.com/83650174/196755341-205ff7e1-b388-4f54-801e-7541b11941a3.png)


Data is collected from Twitter using Twitter-API. The data can be obtained using many search keywords. Once the data is extracted, it is pre-processed to remove hyperlinks and punctuations, symbols, emoticons, etc. using a regular expression to get the clean data. 

Tokenization: Once the data is cleaned and manually labelled, we read the dataset and create tokens (words) by splitting the words from the sentence

Normalization: Normalization helps in reducing the number of unique tokens present in the text, removing the variations in a text, and also cleaning the text by removing redundant information. Here to make the processing easy and we need almost everything from the tweet, we converted the data into lower words

Lemmatization: The tokenized words then need to be converted to their base root form to make sense of each word.

Removal of Stop Words: Stop words are a set of commonly used words in any language. Words like ‘is’, ‘the’, ‘and’ are treated as stop words. In Natural language processing, analysis is based on the important words by removing stop words. For this study, Natural language tool kit (NLTK) and SPACY stop word libraries are used to remove the stop words. Further, the new corpus of stop words are added to the list and appended to the NLTK library. The stop words are removed from the word dictionary. 

Emotion Lexicon: NRC emotion Lexicon is used on the word dictionary to identify the emotions from the word-emotion association provided by the NRC lexicon. Similarly, the words are also passed toward text2motion to identify the emotions of each tweet. Emotion classification and frequencies of emotions are identified from the analysis.
