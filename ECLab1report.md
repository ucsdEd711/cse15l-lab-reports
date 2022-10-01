Edwin’s Lab 1 report 

Installing visual studio code:
Click this URL: https://code.visualstudio.com/ and follow the instruction to download Visual studio code. After downloading, open Visual studio code on your computer and it should look like this.(Check first screenshot)


Remotely connecting:
Remember your CSE username and password.
Open visual studio.
If you have a Mac go to the terminal and then the new terminal.
Enter ssh youraccountname@ieng6.ucsd.edu
Enter your password, after that it should look like this.
Check the second screenshot.

 


Trying Some Commands:
There are a lot of commands you can try, including cd, ls, pwd, mkdir, and cp.
Try to run some commands and understand what those commands do.
For example, The first command ls is to list a file..
The second command cd perl5  is to take you to the directory you want to go to.
The third command cd ~ takes you back to your original directory
The fourth command pwd writes to standard output the full path name of your current directory. 
The fifth command touch is to create a file with the filename you provide.
Check The third screenshot

Moving Files with scp
Log out from your ieng6 by typing exit in the terminal.
Type javac WhereAmI.java, if it counters the error I got “ The operation couldn’t be completed. Unable to locate a Java Runtime that supports javac.Please visit http://www.java.com for information on installing Java.” Then you need to install java and the full JDK package.
After downloading, when you type in javac WhereAmI.java and java WhereAmI, it should look like the screenshot below.
Type in scp WhereAmI.java youraccountname@ieng6.ucsd.edu:~/ and log in to your ieng6 with ssh again.
Type ls you should see WhereAmI.java in there.(second screenshot in this section.)
Log out again by typing exit.
Check the fourth, fifth and sixth screenshots
 


Setting an SSH Key:
Type in ssh-keygen.
Copy the file it provides to be the file to save into
No passphrase for me.
It will show where the public key has been saved, the key fingerprint and the randomart image.( First screenshot in the section)
Type in scp /Users/edwinchen/.ssh/id_rsa.pub cs15lfa22ep@ieng6.ucsd.edu:~/.ssh/authorized_keys, but remember to use the your file and the account name. ( Second screenshot in the section.) 
It will tell you to type in the password for the last time and when you try to log in with ssh again, it won’t ask for the password anymore. 
Check the 7th and 8th screenshot.


Optimizing Remote Running:
Try some commands using remote running. But remember to log out from ieng6 first! 
 Type in ssh cs15lfa22ep@ieng6.ucsd.edu "ls", with your own account name. 
 Type in cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI.
The result should be very similar to the output in the screenshot below.
Check the ninth screenshot
 

