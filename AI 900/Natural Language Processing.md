# Natural Language Processing

**TEXT ANALYSIS**

**Corpus** = a body of text

### Tokenization

### Term Frequency – Inverse Document Frequency (TF-IDF)
Term frequency - inverse document frequency (TF-IDF) is a common technique in which a score is calculated based on how often a word or term appears in one document compared to its more general frequency across the entire collection of documents.

---

## ML FOR TEXT CLASSIFICATION

A common application of this technique is to train a model that classifies text as positive or negative in order to perform sentiment analysis or opinion mining.

---

## SEMANTIC LANGUAGE MODELS

Common NLP tasks supported by language models include:
- Text analysis, such as extracting key terms or identifying named entities in text.
- Sentiment analysis and opinion mining to categorize text as positive or negative.
- Machine translation, in which text is automatically translated from one language to another.
- Summarization, in which the main points of a large body of text are summarized.
- Conversational AI solutions such as bots or digital assistants in which the language model can interpret natural language input and return an appropriate response.

---

## AZURE AI LANGUAGE

### Text Analysis
- **Named entity recognition** identifies people, places, events, and more. This feature can also be customized to extract custom categories.
- **Entity linking** identifies known entities together with a link to Wikipedia.
- **Personal identifying information (PII) detection** identifies personally sensitive information, including personal health information (PHI).
- **Language detection** identifies the language of the text and returns a language code such as `"en"` for English.
- **Sentiment analysis and opinion mining** identifies whether text is positive or negative.
- **Summarization** summarizes text by identifying the most important information.
- **Key phrase extraction** lists the main concepts from unstructured text.

---

## AZURE AI SPEECH

---

## QUESTION ANSWERING

---

## AZURE AI BOT SERVICE

---

## CONVERSATIONAL LANGUAGE UNDERSTANDING

- **Utterances**  
  An utterance is an example of something a user might say, and which your application must interpret.

- **Entities**  
  An entity is an item to which an utterance refers.

- **Intents**  
  An intent represents the purpose, or goal, expressed in a user's utterance.

---

## SPEECH

- **Speech recognition** – the ability to detect and interpret spoken input  
- **Speech synthesis** – the ability to generate spoken output  

---

=========================================================================

Vectorization captures semantic relationships between words by assigning them to locations in n-dimensional space.  

**Stemming = Lemmatization**, also known as stemming, normalizes words before counting them.  

Frequency analysis counts how often a word appears in a text.  

N-grams extend frequency analysis to include multi-term phrases.  

Tokenization is part of speech synthesis that involves breaking text into individual words such that each word can be assigned phonetic sounds.

---

----------------------------------------------------

### [Which two features of Azure AI Services allow you to identify issues from support question data, as well as identify any people and products that are mentioned?]

- **Key phrase extraction** is used to extract key phrases to identify the main concepts in a text. It enables a company to identify the main talking points from the support question data and allows them to identify common issues.  
- **Named entity recognition** can identify and categorize entities in unstructured text, such as people, places, organizations, and quantities.

------------------------------------------

Entity recognition includes the **entity linking** functionality that returns links to external websites to disambiguate terms (entities) identified in a text.

Entity linking identifies and disambiguates the identity of entities found in a text.  
Named entity recognition cannot provide a link for each entity to view further information.

**Content Moderator** is an Azure AI Services service that is used to check text, image, and video content for material that is potentially offensive.

**Personal Identifiable Information (PII)**

Language Name, ISO 6391 Code, and Score are three values returned by the Language service of natural language processing (NLP) in Azure.  
Bounding box coordinates are returned by the Azure AI Vision services in Azure.  
Wikipedia URL is one of potential values returned by entity linking of entity recognition.

Azure AI Language detection identifies the language in which text is written.

Sentiment analysis evaluates text and returns sentiment scores and labels for each sentence.  
Sentiment analysis is used to return a numeric value based on the analysis of a text.

-------------------------------------------------------------------

### [For which two scenarios is the Universal Language Model used by the speech-to-text API optimized?]

- conversational  
- dictation  

The acoustic, language, and pronunciation scenarios require developing your own model.

-------------------------------------------------------------------

Extracting key phrases from text to identify the main terms is an NLP workload.  

Predicting whether customers are likely to buy a product based on previous purchases requires the development of a machine learning model.

Removing stop words is the first step in the statistical analysis of terms used in a text in the context of NLP.  

Counting the occurrences of each word takes place after stop words are removed.  

Creating a vectorized model is not part of statistical analysis. It is used to capture the semantic relationship between words.  

Encoding words as numeric features is not part of statistical analysis. It is frequently used in sentiment analysis.

A webpage or an existing document, such as a text file containing question and answer pairs, can be used to generate a knowledge base.  
You can also manually enter the knowledge base question-and-answer pairs.  
You cannot directly use an image or an audio file to import a knowledge base.

---
