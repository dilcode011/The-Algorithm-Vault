# Text Preprocessing in NLP

## 1. The Concept
Before a computer can understand text, we have to break it down, clean it up, and standardize it. Raw text from the internet is full of punctuation, uppercase/lowercase inconsistencies, and words that don't add much meaning.

Text Preprocessing is the pipeline we use to clean this data.

## 2. The Core Pipeline

### A. Tokenization
The process of breaking a large paragraph of text into smaller pieces called **Tokens**.
* **Sentence Tokenization:** Splitting a paragraph into a list of sentences.
* **Word Tokenization:** Splitting a sentence into a list of individual words.

### B. Stopword Removal
"Stopwords" are the most common words in a language (e.g., "the", "is", "in", "and"). While they are necessary for grammar, they usually carry very little actual meaning for a Machine Learning model. We generally remove them to save processing power and reduce noise.

### C. Stemming vs. Lemmatization
Words often appear in different forms (e.g., *run, running, ran*). We want the computer to know these are all the same core word.

* **Stemming (The Butcher):** A crude, rule-based approach that just chops the end off a word. 
  * *Example:* "Caring" -> "Car" (It makes mistakes!)
  * *Pros:* Very fast.
  * *Cons:* Often creates non-words.
* **Lemmatization (The Linguist):** Uses a dictionary to look up the grammatical root of a word (the Lemma).
  * *Example:* "Caring" -> "Care" / "Better" -> "Good"
  * *Pros:* Accurate and creates real words.
  * *Cons:* Slower than stemming.

## 3. Resources
### 📖 Documentation
* [NLTK (Natural Language Toolkit) Book](https://www.nltk.org/book/)
* [SpaCy 101: Everything you need to know](https://spacy.io/usage/spacy-101)

### 📺 Videos
* [StatQuest: Word2Vec and Text Preprocessing](https://www.youtube.com/watch?v=viZrOnJclY0)