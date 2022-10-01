# Edwin’s Lab 1 report 
We use the Remote Access and the Filesystem to get access to other computer. There are 6 big steps you need to finish.
# Installing visual studio code:
1. Click this URL: https://code.visualstudio.com/ and follow the instruction to download Visual studio code. After downloading, open Visual studio code on your computer and it should look like this.(Check first screenshot)

![Image](ScreenShot1.png)

# Remotely connecting:
1. Remember your CSE username and password.

2. Open visual studio.

3. If you have a Mac go to the terminal and then the new terminal.
4. Enter ssh youraccountname@ieng6.ucsd.edu
5. Enter your password, after that it should look like this.
6. Check the second screenshot.
![Image](ScreenShot2.png)
 


# Trying Some Commands:
1. There are a lot of commands you can try, including cd, ls, pwd, mkdir, and cp.
Try to run some commands and understand what those commands do.
2. For example, The first command ls is to list a file..
3. The second command cd perl5  is to take you to the directory you want to go to.
4. The third command cd ~ takes you back to your original directory
5. The fourth command pwd writes to standard output the full path name of your current directory. 
6. The fifth command touch is to create a file with the filename you provide.
7. Check The third screenshot
![Image](ScreenShot3.png)

# Moving Files with scp
1. Log out from your ieng6 by typing exit in the terminal.
2. Type javac WhereAmI.java, if it counters the error I got “ The operation couldn’t be completed. Unable to locate a Java Runtime that supports javac.Please visit http://www.java.com for information on installing Java.” Then you need to install java and the full JDK package.
3. After downloading, when you type in javac WhereAmI.java and java WhereAmI, it should look like the screenshot below.
4. Type in scp WhereAmI.java youraccountname@ieng6.ucsd.edu:~/ and log in to your ieng6 with ssh again.
5. Type ls you should see WhereAmI.java in there.(second screenshot in this section.)
6. Log out again by typing exit.
7. Check the fourth, fifth and sixth screenshots
 ![Image](ScreenShot4.png)
 ![Image](ScreenShot5.png)
 ![Image](ScreenShot6.png)


# Setting an SSH Key:
1. Type in ssh-keygen.
2. Copy the file it provides to be the file to save into
3. No passphrase for me.
4. It will show where the public key has been saved, the key fingerprint and the randomart image.( First screenshot in the section)
5. Type in scp /Users/edwinchen/.ssh/id_rsa.pub cs15lfa22ep@ieng6.ucsd.edu:~/.ssh/authorized_keys, but remember to use the your file and the account name. ( Second screenshot in the section.) 
6. It will tell you to type in the password for the last time and when you try to log in with ssh again, it won’t ask for the password anymore. 
7. Check the 7th and 8th screenshot.
![Image](ScreenShot7.png)
![Image](ScreenShot8.png)
# Optimizing Remote Running:
1. Try some commands using remote running. But remember to log out from ieng6 first! 
2. Type in ssh cs15lfa22ep@ieng6.ucsd.edu "ls", with your own account name. 
3. Type in cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI.
4. The result should be very similar to the output in the screenshot below.
5. Check the ninth screenshot
 
![Image](ScreenShot9.png)
