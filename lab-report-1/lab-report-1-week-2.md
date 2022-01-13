# Lab Report 1 - Week 2

![Image](labreport1picture1.PNG)
* I had already installed VS Code last quarter for CSE11. I did so by going to the VS Code web page and downloading it for Windows.

---
![Image](labreport1pic2.PNG)
* In order to remotely connect, I had to first find my course specific account for CSE 15L by going to [this website](https://sdacs.ucsd.edu/~icc/index.php). I then typed in the command “ssh (my account address)” and it prompted me to accept or decline and then enter my password.
---
![Image](labreport1pic3.PNG)
* Here, I tested out commands on the remote server. I tested the ls command, which tries to open the specified directory. I also tried cp, which tries to open a file for reading, and cat, which puts the specified file into the terminal.
---
![Image](labreport1pic4.PNG)
* Here, I tested the scp command which copied a file into the remote server. Type “scp”, then the name of the file you are trying to move, and then the user address. It prompted me for a password and then once I typed the password in, the file was successfully copied over.
---
![Image](labreport1pic5.PNG)
* On a Windows PC, in order to set an SSH key so you do not have to enter a password anymore, I had to first type “ssh-keygen -t ed25519” and when prompted for a password, I left it empty, which generated a public and private key.  I then restarted VS code as administrator, and started the ssh agent service and did “ssh-add (name of directory of the private key in my local files)” to add my private key into the service. After this, I used scp to copy the directory of the public key into the remote server.
---
![Image](labreport1pic6.PNG)
* Here is the fastest way I could copy a file onto the remote server and run it from there. After removing some lines of code from the WhereAmI.java file on my local computer, I first ran the scp command to copy the file to the remote server, and by adding a semicolon I could run the ssh line on the same command. By having “javac WhereAmI.java; javaWhereAmI” this both compiles and runs the file on the remote server and then logs out and returns to my local machine.
