# CSE 15L Lab Report-week 1
## how to log into a course-specific account on `ieng6`
## __Step1: install Visual Studio code__
Google vscode download and select the download package corresponding to your OS  
![image](DownloadPage.jpg)
Open VScode, you should be at a home page like this.  
Depending on the default theme setting, it could be white.
![image](vscode_home.jpg)
## __Step2: connect to remote ieng6 sever__
First, you need to look up your ieng6 account name at [here](https://sdacs.ucsd.edu/~icc/index.php).    
Follow the instructions there to reset your account's password, so that your `ieng6` account can be activated.Take a note of your new password. It's needed for remote server login.

After resetting your password, open terminal in VScode by clicking "Terminal"-"New Terminal",and type in the following command with `zz` replaced by letters in your course-specific account.  
$ ssh cs15lwi22zz@ieng6.ucsd.edu  
For all yes/no questions poping up, type yes.  
e.g.:  
`The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?`  

Type in your new password you just reset when `Password:` appears, and you should have logged into your remote `ieng6` server.  
__Note:__ 
![image](remote-login.jpg)
