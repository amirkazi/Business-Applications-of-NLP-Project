# Analyzing 2013 Election Manifestos for Pakistani Political Parties through Natural Language Processing

## Goal:
- Analyzing 2013 election manifestos for 6 different Pakistani political parties, to understand policy stances, issue prioritization etc.
- Visualizing key areas for voter assistance, such as creating Word Clouds to highlight most frequent high priority words in each manifesto, plotting manifesto sentiment graphs indicating 'doom and gloom' vs 'optimism and hope' strategies for each party.
- Doing a proxy test for the 'Median Voter Theorem' by analyzing text similarity across different manifestos, to see how different parties are - at least in how they portray themselves in their manifestos. 

## Content:

#### Manifesto Source Files Folder:
- Source files for PPP, ANP, MQM and PTI were taken from: http://www.cpdi-pakistan.org/party-manifestos 
- The previous source was not used for PMLN and JI because their files in that source comprised of images instead of text.
- Source file for PMLN is from: 
http://pmo.gov.pk/documents/manifesto.pdf
- The above files were converted to txt format through a website called:
http://pdf2doc.com 
- Source file of Ji is from:
https://kurzman.unc.edu/files/2011/06/JI_2013_English.pdf
This file was an image file and had to be converted to txt through ‘Optical Character Recognition’. As such, this file contains some errors.
  
#### Manifesto Text Files Folder:
- Contains the text files (converted) which will be used for analysis.


#### Code File:

##### The code does the following things:
- Reads each Manifesto text file and creates a ‘Manifesto’ Class (Object Oriented Programming)
- Creates Word Tokens 
- Creates Sentence Tokens 
- Finds Word Frequency in each text file 
- Parts of Speech tagging 
- Creates a 'stemmed list' for the tokens 
- Pre-processes to remove stop words & converts to lower case to avoid repetition
- Finds any top K number of most frequent words in each text file
- Creates a word cloud of any given text, for any optional number of words
- Summarizes text from any text file
- Creates n-grams of any length, and presents any X most common n-grams
- Calculates document similarity between any two manifestos
- Calculates sentence sentiment (polarity & subjectivity) & plots sentiment graphs

##### The following Python packages were used in this program:
- NLTK
- Gensim
- Word Cloud
- Matplotlib
- Collections
- Spacy
- TextBlob


Done As:
Final project for UChicago Booth course 'Business Applications of Natural Language Processing' Spring 2018
