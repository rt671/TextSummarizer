# TextSummarizer
## Description
- Text summarization is the process of creating a brief, coherent, and fluent summary of a longer text document, which involves highlighting the text's crucial informative aspects and content meaning.
- There are two approaches to text summarization: Extractive and Abstractive. In the Extractive approach, a summarizer tries to find and combine the most significant sentences of the corpus to form a summary whereas Abstractive text summarization is the process of extracting the most important meaning from a text and rewriting it in a summary.
- Used the extractive approach and tried to summarize the text on a lexical level. NLTK library is used for cleaning the data to remove the non-essential words and finding the appropriate words on the basis of their frequency and syntactic arrangement.
- Created a web app as an interface where the user adds the text and obtains the summary. This is done with the help of streamlit library which is an open source Python library for creating custom web apps for ML and Data Science applications. 

## Workflow:
- Data Cleaning: Removing some particular characters which hold trivial meanings for creating a summary. This is done with the help of regular expressions which are used for pattern matching and searching. They include all the special characters, extra spaces, single-character words, characters in square brackets (they indicate references), and more. 
- Initially, all the words are converted into lowercase. If the word is present in the stopword list then it is removed, else the frequency of the word is increased by 1.
- Next relative frequencies of each word are calculated and corresponding weights are assigned to them. This will let us proceed to find the sentence scores. 
- Eventually using a heap a few sentences are selected with the maximum score and are concatenated to produce the summary.

## Output:
![image](https://github.com/rt671/TextSummarizer/assets/82562103/b9430e82-a2ea-4685-b517-24ec489aff03)
