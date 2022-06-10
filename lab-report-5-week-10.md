# Lab Report 5
## Week 10

# Finding tests with different results 
I was able to find tests with different results by using `vimdiff` on the results of `script.sh`. I used the steps from Lab 9 to redirect the results of the `script.sh`. I ran the command `bash script.sh > results.txt` in the implementation provided in lab 9 and my group's representative implementation. Once I had two `results.txt` files, one from the provided implementation and one from a representative of my group. I ran `vimdiff cse15lsp22-markdown-parser/results.txt wk-5-parse/results.txt` to compare results of each test. 
* After running `vimdiff` I found differences in:
    * test-files/14.md [link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/14.md)
    * test-files/472.md [link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/472.md)

# Test One 
* `vimdiff` results
![Image](test-files-472.png)
* Implementation from lab 9 
    * ![Image](cs15l-14.png)
* Group Representative implementation 
    * ![Image](group-14.png)
