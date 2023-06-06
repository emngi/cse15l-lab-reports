### Lab Report 5
#### Student Query:
![Image](/lab5/s1.png)
---
#### TA response:
![Image](/lab5/s2.png)
Additional Information:
![Image](/lab5/s3.png)
![Image](/lab5/s4.png)
![Image](/lab5/s5.png)
---
The file and directory structure was pulled from week 7's lab. This contained the files of ListExamples.java, ListExamplesTests.java, test.sh, and the jUnit files.
Contents of test.sh file before fixing the bug:
![Image](/lab5/s6.png)
- The command I used to trigger the bug was `bash test.sh <enter>`
- The student was first prompted to change the commands from
`javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java`
`java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore ArrayTests`
to the Mac OS commands:
`javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`
`java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ArrayTests`
- then they were promted to update the `ArrayTest` part to the correct parameter being `ListExamplesTests`
### Part 2 -- Reflection
- Throughout the second half of this quarter something I found interesting was vim. It didn't occur to me that there would be a need to update files remotely or in that manner. Learning about vim and remote server in general was very interesting. It was cool how we were editing files on the ieng6 accounts. And how we were able to change the files and push updates. I found this interesting because I used to use github as a kid to download mods for minecraft or othervideo games and now I know how it works.
