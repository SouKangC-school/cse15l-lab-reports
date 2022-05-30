# Introduction
For this lab report, I would add a test both to my implementation markdown-parse, and the implementation I reviewed in week 7 for each of the three snippets provided in the instruction. I would run the tests and show the reults of running the tests on each.  

---

# Link to Respository
1. [link](https://github.com/SouKangC-school/markdown-parser-a) to my implementation
2. [link]() to reviewed group's implementation

# For each test
## Snippet 1
1. Expected output

["`google.com", "google.com", "ucsd.edu"]

2. My implementation
* Code
![image](image-4\4.1.png)
* Junit output
![image](image-4\4.2.png)

3. Reviwed group's implementation
* Code
![image](image-4\4.3.png)
* Junit output
![image](image-4\4.4.png)

## Snippet 2
1. Expected output

["a.com", "a.com(())", "example.com"]

2. My implementation
* Code
![image](image-4\4.5.png)
* Junit output
![image](image-4\4.6.png)

3. Reviwed group's implementation
* Code
![image](image-4\4.7.png)
* Junit output
![image](image-4\4.4.png)

## Snippet 3
1. Expected output

["https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule"]

2. My implementation
* Code
![image](image-4\4.8.png)
* Junit output
![image](image-4\4.9.png)

3. Reviwed group's implementation
* Code
![image](image-4\4.10.png)
* Junit output
![image](image-4\4.4.png)

# Answer to questions
> Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

> A: I think it only requires a small code change that would make my programe work for all related cases to inline code with backticks. Some specifications over the inclusion of backticks should be added over to the logistics behind locating left and right parenthesis and determining if a link exist. Overall, no major change of code is needed at least from my expectation.  

---

> Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

> A: No, I do not think there exists a small code change solution that make my programe compatible with related cases that include nest parentheses, brackets, and escaped brackets. Such reassurance comes from the fact that I have tried modifying the code myself in hope of making it pass through a related case before and it did not work out very easily. Another reason is that the correct solution ,according to my instructor, to related cases like this seems to be very different from what I have for now, meaning that it is unlikely that a small code change would be enough to make the entire programe work.  

---

> Q: Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

> A: Honestly I am not too certain about this question due to the fact that I am receiving a index-out-of-bound error that I have not figured out the rationale behind. I am more inclined to believe that there would not be a small code change solution to such error as it is already quite hard for me to locate the error in the first place. I am guessing there is something wrong with the process of index variables such that when new lines are encountered some inproper logisitcs would turn the variables into invalide ones that trigger the index-out-of-bound exception somewhere in the programe. 