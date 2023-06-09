# Lab Report 4
---

## 1. Log into ieng6

   * I used `Ctrl + C` and `Ctrl + V` to copy credentials from notes. This step logs into the remote account.
  ``` java
  $ ssh cs15lsp23cw@ieng6.ucsd.edu <Enter>
  (cs15lsp23cw@ieng6.ucsd.edu) Password: <Paste or type password and hit Enter>
  ```
  ![Image](step1.png)
  
---
  
## 2. Clone your fork of the repository from your Github account
   * I used `Ctrl + C` and `Ctrl + V` to copy this command from the lab write up. `git clone` clones the entire repo into my remote account.
``` java
$ git clone https://github.com/emngi/lab7.git <Enter>
```
![Image](lab4/step2.png)
---
## 3. Run the tests, demonstrating that they fail
   * I used `<tab>` to autocomplete t into `test.sh`. CD changed the directory I was in and bash ran the commands in the file test.sh.
```java
$ cd lab7 <Enter>
$ bash t<Tab> <Enter>
```
![Image](lab4/step3.png)
--- 
## 4. Edit the code file to fix the failing test
   * I use `<tab>` twice to autofill L to `ListExamples.java`. Using vim as an editor, `/index1` searches for all instances of index1. n and l are used to move around the file and then I used r 2 to replace the 1 with 2. ESC ensures you are in normal mode and :wq saves and exit.
```java
$ vim L<tab>.j<tab> <Enter>
$ /index1 <Enter> n n n n n n n n n l l l l l r 2 <Esc> :wq
```
![Image](lab4/step4.png)
  
--- 
  
## 5. Run the tests, demonstrating that they now succeed
  * bash runs the tests in the test.sh file
`$ bash t<tab>`
  
![Image](lab4/step5.png)
  
---
  
## 6. Commit and push the resulting change to your Github account (you can pick any commit message!)
   * I use `<tab>` twice to autofill L to `ListExamples.java`. `git add` adds ListExamples.java to what is going to be committing, `git commit` commits it.  
  ```java
  $ git add L<Tab>.j<Tab> <Enter>
  $ git commit -m Done! <Enter>
  $ git push origin
 ```
![Image](lab4/step6.png)
  
