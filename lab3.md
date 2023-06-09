# Lab Report 3
I chose the find command. This command searches for files within a directory of folder. It's very useful when searching for a specific file in a large repository.

1. `-size` (search by file size) | [Source](http://linuxcommand.org/lc3_man_pages/find1.html) 
- This option searches for files that match the specified size.
- Example 1
  -  This example is searching for files bigger than 100 KB in the technical directory and its subdirectories. It's useful because you might not want to see small or big files depending on your needs.
```java
$ find technical -type f -size +100k
technical/911report/chapter-1.txt
technical/911report/chapter-12.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-3.txt
technical/911report/chapter-6.txt
technical/911report/chapter-7.txt
technical/911report/chapter-9.txt
technical/biomed/1471-2105-3-2.txt
technical/government/About_LSC/State_Planning_Report.txt
technical/government/About_LSC/commission_report.txt
technical/government/Env_Prot_Agen/bill.txt
technical/government/Env_Prot_Agen/ctm4-10.txt
technical/government/Env_Prot_Agen/multi102902.txt
technical/government/Env_Prot_Agen/tech_adden.txt
technical/government/Gen_Account_Office/GovernmentAuditingStandards_yb2002ed.txt
technical/government/Gen_Account_Office/May1998_ai98068.txt
technical/government/Gen_Account_Office/Sept27-2002_d02966.txt
technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt
technical/government/Gen_Account_Office/ai9868.txt
technical/government/Gen_Account_Office/d01376g.txt
technical/government/Gen_Account_Office/d01591sp.txt
technical/government/Gen_Account_Office/d0269g.txt
technical/government/Gen_Account_Office/d02701.txt
technical/government/Gen_Account_Office/gg96118.txt
technical/government/Gen_Account_Office/im814.txt
technical/government/Gen_Account_Office/pe1019.txt
```
- Example 2
  -This example is useful for looking for small files, this one is looking at files less than 3KBs.
```java
$ find technical -type f -size -3k 
technical/government/Media/Campaign_Pays.txt
technical/government/Media/Court_Keeps_Judge_From.txt
technical/government/Media/Fire_Victims_Sue.txt
technical/government/Media/Helping_Hands.txt
technical/government/Media/It_Pays_to_Know.txt
technical/government/Media/Justice_requests.txt
technical/government/Media/Lawyer_Web_Survey.txt
technical/government/Media/Self-Help_Website.txt
technical/government/Media/Wilmington_lawyer.txt
technical/plos/pmed.0020028.txt
technical/plos/pmed.0020048.txt
technical/plos/pmed.0020082.txt
technical/plos/pmed.0020120.txt
technical/plos/pmed.0020157.txt
technical/plos/pmed.0020191.txt
technical/plos/pmed.0020192.txt
technical/plos/pmed.0020226.txt
```
2. `-mtime` (search by modification time) | [Source](http://linuxcommand.org/lc3_man_pages/find1.html) 
- This option searches for files that have been modified within the specified time frame.
- Example 1
  -  This example searches for any files modified within the last 7 days. This is useful for finding recently modified files. It returned nothing since nothing had been modified within the specified timeframe.
 ``` java
 $ find technical -type f -mtime -7
```
- Example 2
  - This example searched for files modified more than 30 days ago in the technical directory and its subdirectories. Again returned nothing. So given these two results everting has been modified within the last 30 days but not since a week.
``` java
$ find technical -type f -mtime +30
```
3. `-name` (search by file name) | [Source](http://linuxcommand.org/lc3_man_pages/find1.html) 
- This option searches for files or directories that match the specified name.
- Example 1
  - This example searches for any .txt files that end with economy. This might be useful to find similar files and if you dont fully remembe the file's name.
```java
$ find -name "*_economy.txt"
./technical/government/Media/Weak_economy.txt
```
- Example 2
  - This example searches for any.txt files starting with chapter. This is useful to see all chapters listed out.
```java
$ find -name "chapter*.txt"
./technical/911report/chapter-1.txt
./technical/911report/chapter-10.txt
./technical/911report/chapter-11.txt
./technical/911report/chapter-12.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-2.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-5.txt
./technical/911report/chapter-6.txt
./technical/911report/chapter-7.txt
./technical/911report/chapter-8.txt
./technical/911report/chapter-9.txt
```
4. -user (search by file owner) | [Source](http://linuxcommand.org/lc3_man_pages/find1.html) 
- This option searches for files that are owned by the specified user.
- Example 1
  -  This example searches for files owned by user "emily". No files returned. This is useful if you have many different user's files in a directory.
```java
$ find technical  -user emily
find: 'emily' is not the name of a known user
```
- Example 2
  - This example searches for files owned by the user "jpolitz". No files returned. Again useful for finding a specific user's files, especially when there are a lot of collaborators like in this class.
```java
$ find technical  -user jpolitz   
find: 'jpolitz' is not the name of a known user
```
