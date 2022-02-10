
# Lab Report 3 - Week 6

## Copy whole directories with scp -r

![Image](lab3pic1.PNG)
* Copying my whole markdown-parse directory to your ieng6 account using the command `scp -r *.java *.md lib/ C:\Users\clair\OneDrive\Documents\GitHub\markdown-parse\Makefile  cs15lwi22adh@ieng6.ucsd.edu:markdown-parse`
* This command adds the whole directory and also the Makefile

![Image](lab3pic2.PNG)
![Image](lab3pic3.PNG)
* The command `ssh` allows me to log in to my ieng6 account
* The command `cd` allows me to change my directory to the markdown-parse directory

![Image](lab3pic4.PNG)
* Compiling and running the MarkdownParseTest file in the remote server

![Image](lab3pic6.PNG)
* Copying the whole directory and running the tests on one line using `ssh`, `scp`, `cd`, and `;`