#                                                         WEEK 2 Lab Report

**Installing VScode**
* Go to the website https://code.visualstudio.com, and download the correct version for your operating system.
* After you download and install the VScode, you will see the following iamge:
* <img width="770" alt="image steP1" src="https://user-images.githubusercontent.com/103226676/162665848-7117cbe0-ccf9-4613-b0ed-6eaef912c8e0.png">


**Remotely Connecting**
* Follow this link https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse to Install  OpenSSH in order to connect your computer to other computers.
* Here is the link to learn how to connect to a remote computer https://code.visualstudio.com/docs/remote/ssh#_connect-to-a-remote-host
* The first step is to open a new terminal and type the folling code `$ ssh cs15lsp22zz@ieng6.ucsd.edu` to coonect ucsd ieng6 computer, but you need to change the zz to a specific account.
* If it the first time you will see the following output on your laptop
```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't
be established.
RSA key fingerprint is
SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting
(yes/no/[fingerprint])?
```
* You should type "yes" and press "enter", then give your password to login. 
* Then you successfully connect to the remote computer and will see the following image:
* <img width="679" alt="image step2" src="https://user-images.githubusercontent.com/103226676/162668053-f542e2a7-9870-48dc-aaf4-fed5b934d4dc.png">


**Trying some command**
* Here are some commands you can try
* `pwd` : print working directory
* `ls` : list files
* `cp` : copy (you need put the directory after cp)
* `mv` : move or rename
* `cd` : change directory
* `mkdir` : make directory
* `rm` : remove
* `cat` : view or create a file (you need to put the direcory and the file's name after cat)
* `touch` : create a file
* `man` : display command manual
<img width="518" alt="image step3" src="https://user-images.githubusercontent.com/103226676/162669593-9ecc6c4f-dda1-43c6-a6ae-b31cc3939777.png">
