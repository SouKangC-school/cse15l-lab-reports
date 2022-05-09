# Introduction
For this lab report, I would implement all Group Choice Opion (1-3) from lab 5. A detailed steps with relevant screenshots and descriptions would be attached below. 

---

# Streamlining ssh Configuration
1. Open `~/.ssh/config` on VS code, add the following lines:
```
Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lsp22zzz (use your username)
```
![Image](image-3\1.1.png)

2. Log into my account using just the alias I chose
![Image](image-3\1.2.png)

3. Use scp command copying a file using just the alias I chose
![Image](image-3\1.3.png)

# Set up Github Access from ieng6
1. Show where the public key I made is stored on Github and in my user account
![Image](image-3\2.1.png)

2. Show where the private key is made is stored on my user account
![Image](image-3\2.2.png)

3. Show running `git` commands to commit and push a change to Github while logged into my ieng6 account
![Image](image-3\2.3.png)

4. Show a link for the resulting commit:
[commit link](https://github.com/SouKangC-school/cse15l-lab-reports/commit/3bc56a836425917c64da9dfb0c796ed20c6fbec3)

# Copy whole directories with `scp -r`

1. Show copying my whole markdown-parse directory to my ieng6 account
![Image](image-3\3.1.png)

2. 