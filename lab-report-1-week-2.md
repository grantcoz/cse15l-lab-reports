# Lab Report 1 week 2

## Installing Vs-code

1. Use this link to be taken to the website to [Install vs-code](https://code.visualstudio.com/)

2. Once you successfully installed vs-code your screen should look like this ![](Captures/Lab-reports/lab-report-1-week-2/Capture1.PNG)

3. Congrats you just installed and ran vs-code

## Remote connecting

1. Before you can remotely access you first need to find out what your username is and change you password. Your username should look like this 'cs15lsp22zz' but the "zzz" should be replaced with a random set of letters.

![](Captures/Lab-reports/lab-report-1-week-2/Capture2.PNG)

2. You can find out what your username is and change you password by using this link. It might take 15 - 20 minutes for your password change to take effect. [Username and password](https://sdacs.ucsd.edu/cgi-bin/alloc-query) 

3. Now that you have changed you password it is now time to try to sign into your account on the server remotely. To do this open your terminal in vs-code. The terminal can be found at the top of vs-code

![](Captures/Lab-reports/lab-report-1-week-2/Capture3.PNG)

4. Once the terminal is open type the command 'ssh' (which stands for secure socket shell) and your username with '@ieng6.ucsd.edu' at the end. ex. 'ssh cs15lsp22zz@ieng6.ucsd.edu'. After you ssh you should be prompted for your password and if you successfully logged in then you screen should look like this.

![](Captures/Lab-reports/lab-report-1-week-2/Capture4.PNG)

## Trying Some Commands

- When in the terminal there are various commands that can help. Try some commands and see what they do. Here is a list of some commands that you should try.

1. ls
2. ls -a
3. ls -l
4. ls -t
5. ls -lat
6. pwd
7. cd 
8. cd ..
9. cd ~
10. clear

- There are plenty of other commands to try though. Here is a link for a cheat on some commands. [Linux command cheat sheet](https://linuxconfig.org/linux-commands-cheat-sheet)

![](Captures/Lab-reports/lab-report-1-week-2/Capture5.PNG)

## Moving Files with scp

1. For this next part we will be transfering a file from our client computer to the server. Copy this code, create a new file, and name the file WhereAmI.java

`class WhereAmI {
    public static void main(String[] args) {
        System.out.println(System.getProperty("os.name"));
        System.out.println(System.getProperty("user.name"));
        System.out.println(System.getProperty("user.home"));
        System.out.println(System.getProperty("user.dir"));
    }
}`

2. If you have java installed you can run this code in the terminal by using 'javac WhereAmI.java' to compile the code and 'java WhereAmI.java' to run the code. The output of this code should look similar to this.

![](Captures/Lab-reports/lab-report-1-week-2/Capture6.PNG)

3. Once you have you the file created you can now copy over your file to the server by using `scp` which stands for secure copy. 



## Setting an SSH Key
## Optimizing Remote Running