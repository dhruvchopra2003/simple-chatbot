# simple-chatbot
simple rule based chatbot made using scikit and NLTK

The project was built in python, using the libraries numpy(for math functions and arrays), pandas(to handle tables), NLTK(the natural language toolkit), string and random.
The project is based on Natural language processing, an integral part of deep learning.

# A little about the chatbot:
A chatbot or chatterbot is a software application used to conduct an on-line chat conversation via text or text-to-speech, in lieu of providing direct contact with a live human agent. A chatbot is a type of software that can help customers by automating conversations and interact with them through messaging platforms.

This particular chatbot acts upon a fixed data that has to be provided to it beforehand, I recommend creating a data.txt file which contains a sample text, eg copied from any webpage on the internet. The chatbot would be able to traverse through the contents of that file and be able to return relevant phrases and text according to the user input.

### How to build?
For this little chatbot, I have used the Punkt Tokenizer, and the wordnet dictionary, both of them are included in the NLTK library that you previously imported, although you might have to download them using nltk.download().

# Text-preprocessing
The process begins with tokenzing the raw doc into a list of sentences and further into a list of words.
Next comes the text preprocessing , using the nltk.stem.WordNetLemmatizer() command. WordNet is a semantically- oriented dictionary of English which comes included with the NLTK library. This was a step called Lemmatization, a process in which we group together different forms of a word, so that the computer reads it as the same word, and groups together similar meaning words.

# Greeting
Next comes the part of the chatbot, that the users will see, it's responses, and since we are building a well-mannered chatbot, we will include a greeting function.
The greeting function, would just have two lists, one of the user input(eg. Hi, hello) and the other for the chatbot output (eg. welcome, hi there). A simple loop just to identify these words in a sentence and returning a random index from the second list would complete thif function!

# Conversation
The conversation takes place within a loop, until the user mentions the words, "thanks" or "GoodBye", which would trigger the concluding remarks from the chatbot and the conversation would come to an end. During the runtime of the loop, the user can type in any keyword or ask simply framed questions, in order to get the best answers. Since the chatbot is very basic, it will parse through it's knowledge base to find the tokens that the user has input, and then try to find the optimal solution withing the shortest possible time. 

