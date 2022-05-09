# Lab Report 3  
## Week 6

# Streamlining ssh Configuration 
 * I acessed my `.ssh/config` file by creating the file by using vim. 
 ![Image](vim-ssh.png)
 * I edited the file using vim. 
 ![Image](vim-config-edit.png)
    * Once I made these changes, I was able to log into my remote account by using the command `ssh ieng6`
        * ![Image](ssh-ieng6.png)
 * `scp` command 
    * I first created a local directory and file by using `vim ~/lab5A/test.txt`
    * I also created a remote directory so the file could have a destination. I logged on by `ssh ieng6` and created a directory `mkdir week6`
        * ![Image](mkdir-wk6.png)
    * Copied test.txt from local machine to remote machine
        * `scp lab5A/* ieng6:~/week6`

    ![Image](scpLab5A.png)

# Setup Github Access from ieng6
* Once I had a copy of my public key, I copied it into my github account to make a new ssh key.
![Image](keygen-exists.png)
    * `cat ~/.ssh/id_rsa.pub` to print out the key in terminal 

* ![Image](github-keygen.png)
    * I made a SSH key for my personal laptop and my remote CSE 15L account

# Copy whole directories with `scp -r`
* Copied my whole markdown-parse directory to my ieng6 account 
![Image](scp-r.png)
![Image](scp-r2.png)
* Markdown-parse is successfully copied, as it shows up on my remote machine. 
![Image](remote-mdp.png)
* Compiling and running the tests for markdown-parse on my remote ieng6 account 
* ![Image](remote-md-run.png)