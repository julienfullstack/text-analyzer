_Text Analyzer_
#### By _Julien Lenaz_
#### _Website which analyzes text based on user input_
[GitHub Repo](https://github.com/julienlen/text-analyzer/)
## Technologies used:
*_HTML_
*_CSS_
*_Javascript_
*_Git_
## Description
A simple website which counts the words inputted by the user
## Set up
*_Open folder in code editer OR_
*_Run in any browser*
_It's really that simple_

## Known Bugs
* _No known bugs_
* 
## License

_[MIT](https://choosealicense.com/licenses/mit/)_

Copyright (c) _2023_ _Julien Lenaz_ 

##Pseudocode tests

Describe: wordCounter()

Test: "It should return 1 if a passage has just one word."
Code:
const text = "hello";
wordCounter(text);
Expected Output: 1

Test: "It should return 2 if a passage has two words."
Code:
const text = "hello there";
wordCounter(text);
Expected Output: 2

Test: "It should return 0 for an empty string."
Code: wordCounter("");
Expected Output: 0

Test: "It should return 0 for a string that is only spaces."
Code: wordCounter("            ");
Expected Output: 0

Test: "It should not count numbers as words."
Code: wordCounter("hi there 77 19");
Expected Output: 2

Describe: numberOfOccurrencesInText()

Test: "It should return 0 occurrences of a word for an empty string."
Code: numberOfOccurrencesInText(word, text);
const text = "";
const word = "red";
Expected Output: 0

Test: "It should return 1 occurrence of a word when the word and the text are the same."
Code: numberOfOccurrencesInText(word, text);
const text = "red";
const word = "red";
Expected Output: 1

Test: "It should return 0 occurrences of a word when the word and the text are different."
Code: numberOfOccurrencesInText(word, text);
const text = "red";
const word = "blue";
Expected Output: 0

Test: "It should return the number of occurrences of a word."
Code: numberOfOccurrencesInText(word, text);
const text = "red blue red red red green";
const word = "red";
Expected Output: 4

Test: "It should return a word match regardless of case."
Code: numberOfOccurrencesInText(word, text);
const text = "red RED Red green Green GREEN";
const word = "Red";
Expected Output: 3

Test: "It should return a word match regardless of punctuation."
Code: numberOfOccurrencesInText(word, text);
const text = "Red! Red. I like red, green, and yellow.";
const word = "Red";
Expected Output: 3

Describe: omitSwearWords

Test: "It should omit 'swear words'"
Code: omitSwearWords("text") 
const text = "zoinks, muppeteer, biffaroni, loopdaloop, hello";
const word = "hello"
Expected Output: "hello" 


Test: "It should omit 'swear words' regardless of case"
Code: omitSwearWords("text") 
const text = "zoinks, muppeteer, biffaroni, loopdaloop, hello";
const word = "hello"
Expected Output: "hello" 