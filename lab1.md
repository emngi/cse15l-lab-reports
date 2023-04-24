## Installing VS Code
1. Head to the [VS Code website](https://code.visualstudio.com/)
2. Click on the Download button (make sure it is for the correct operating system)
![Image](<https://github.com/emngi/cse15l-lab-reports/blob/main/vs.png?raw=true>)
4. Follow the directions for the installer!
5. Open the desktop shortcut or where ever you have downloaded the application and enjoy :P

## Remotely Connecting
1. Open the VS code application
2. Open a new terminal by
    - clicking the button at the top right
    ![Image](<https://github.com/emngi/cse15l-lab-reports/blob/main/term.png?raw=true>)
    - using the keyboard shortcut *Ctrl + Shift + `*
    - or navigating the menu bar *Terminal > New Terminal*
3. In the terminal type the following:
`ssh cs15lsp23XX@ieng6.ucsd.edu (Xs should be ur own ID letters)`
4. Answer the prompt yes/no/[fingerprint] *if applicable* 
        - usually you should just have to type in yes once (if prompted to do this on a server you connect to often it might be cause for concern)
6. Enter password *you will not be able to see what you are typing*
7. You should see a succsessful connection in the terminal!

## Trying Commands
1. In a remote or local terminal try using some of the commands we learned in class
    - cat <path 1> <path 2> ... | this command stands for concatenate and can be used to view content of files
    - ls <path> | this command prints a list of everything inside a directory
    - pwd | this command prints the full path name of your current directory 
    - cd <path> | this command can be used to change the current working directory
Some examples of output for the commands are:
![Image](<https://github.com/emngi/cse15l-lab-reports/blob/main/cmds.png?raw=true>)
