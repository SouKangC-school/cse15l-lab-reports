# Introduction
For this lab report, I would choose any two tests from the 652 tests where my implementation had different answers than the implementation we provided for lab 9. The tests with different answers should correspond to different bugs - that is, you couldn' teasily fix boht with one code change. 

---

# How to find the tests with different results
Before looking for the difference, I run `bash script.sh >> results.txt` for both my directory and the provided directory. With the text documents established, I simply run `vimdiff my-markdown-parser.results.txt cse15lsp22-markdown-parser/results.txt` to look for test cases with different outputs. The vim system would highlight them automatically so that I do not have to manually search through.

# Link to the test file with different-results
[194.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md?plain=1)

[201.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md?plain=1)

# For each test
## 1. 194.md
1. The correctness of outputs
The provided implementation demonstrates the correct output
2. The demonstration of outputs
* Actual output:
![image](image-5\5.1.png)
* Expected output: [url]
3. Description of the bug and a possible fix
* Code segment
![image](image-5\5.3.png)
* Solution: In this case, it is my implementation that does not work out correctly. This test case is quite special, as it involves with `:` which I have no clue on its usage back when I was typing the above code segment. Honestly, I am still not sure why url would be considered as a link as though it is divided from `[]` with `:my_`. The only thing I am sure of is that some special modifications should be taken in the above code segment so that the `:` would be treated correclty as we parse the link down. 

## 2. 201.md
1. The correctness of outputs
My implementation demonstrates the correct output
2. The demonstration of outputs
* Actual output:
![image](image-5\5.2.png)
* Expected output: []
3. Description of the bug and a possible fix
* Code segment
![image](image-5\5.4.png)
* Solution: For this test case, it is the provided implementation that produces the wrong output. As you can see, the test 201.md includes `:` as well. But what's different from the previous test 194.md is that the existance of a space right after that `:` sigh. Even though I am not too sure how `:` is used in markdown language, I could deduce that the insertion of space after `:` would cut down the connection between the brackets and parenthesis, preventing a link to be created. As of the actual code change, I believe some modifications should be made around the code segment above as that section of code is mainly in charge of the task of finding the next open parenthesis. 
