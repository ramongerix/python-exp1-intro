## ECE2112 - Introduction to Python
Experiment 1: basic string, list, and function problems.

## Contents
- Variables & Data Types
- Lists, Tuples, and Dictionaries
- Functions
- Input, Output

## Getting Started
1. Download `ECE2112.PA.1.IntroPython.ipynb`
2. Open the file on your **Jupyter Notebook**
3. Run cells

## Requirements 
- VSCode or Jupyter Notebook
- Python 3

💡 *Keep it simple. Run code. Explore. Learn.*  

## Code - Explains 
### 01 🔠 Alphabet Soup Problem
 `def alphabet_soup(word):`
- creates a function named alphabet_soup
- It stores one parameter, a word (str) string.


 `(sorted(word, key=str.lower))`
- **sorted()** takes the string and breaks it into individual characters
- **key=str.lower** ensures sorting is case-insensitive


 `"".join(sorted(word, key=str.lower))`
- **join()** takes the sorted list of characters and combines them back into a single string.


`print(sorted_word)`
- shows the alphabetically sorted version of the input (str) string.


`alphabet_soup("type here")`
- a user or tester of the program will input their chosen text to be arranged alphabetically inside the parentheses, and running the cell will sort it.


### 02 😀 Emoticon Problem
`def emotify(sentence):`
- creates a function named emotify
- it stores one argument, a sentence (str) string.


`emoticons = {"smile":":)", "grin":":D", "sad":":((", "mad":">:("}`
- creates a **dictionary** where; keys are words ("smile", "grin", "sad", "mad") and the values corresponding emoticons (":)", ":D", ":((", ">:("),


`words = sentence.split()`
- **split()** breaks the input string into a list, separating by spaces.
  e.g. "I am sad" -->["I", 'am", "sad"]

`output = [emotions.get(word, word) for word in words]`
- a list
- **emotions.get(word, word)** look up the word in the dictionary
- if it exists it will use the emoticon
- if not it will just keep the original input word.


`return " ".join(output)`
- turns the list back into sentence


`emotify("I am sad")`
- calls the function with the sentence "I am sad"
- it will output "I am :(("










