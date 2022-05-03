# Lab Report 2
## Week 4

# Change 1: No link in the test file 
### Code Change 
![Image](Change1.png)
### Symptom 
![Image](Symptom1.png)
### Link to test file for _failure-inducing input_ 
* [test-file4.md](https://github.com/cindy4127/markdown-parser/commit/dfef581544d69a463027107699984290006f1f0a)
### Explanation
There is no link present in the file. There is just the instructions to copy a link into the file. As a result of there being no links, some variables will not be found while looping through. This will cause an out of bounds error, as the variables are set to -1. In the case of `toReturn.add(markdown.substring(openParen + 1, closeParen));` -1 is substituted for both openParen and closeParen. This attempts to access a substring of size (0,-1), which is invalid. Which is why we see the out of bounds error as our symptom. 

# Change 2: Link contains image reference
### Code Change 
![Image](changes2.png)
### Symptom 
![Image](Symptom2.png)
### Link to test file for _failure-inducing input_ 
* [test-file5.md](https://github.com/cindy4127/markdown-parser/commit/297ec59e7c0751a682842b4f188c56840f517716)
### Explaination 




