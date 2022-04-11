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
  
   
  **Moving file with scp**
  * we can use the scp command to copy a file on your computer to the remote computer. 
  * For exapmle, you can create a WhereAmI.java file and compile it on your device
  * Then under the compile command, you should run `scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/`
  * You should type the same password as your ssh again.
  * Use the ls command, you should see the file and you can run it with the javac java command on the remote device.
  * The following image is a successful example.
  * <img width="457" alt="image step4" src="https://user-images.githubusercontent.com/103226676/162670923-084a1526-2c96-4cf2-b749-dc31a648c30e.png">
   
   
**Setting an SSH key**
* `ssh keygen` creats the public key file and private key files. You can save the public key in a location on the server and private keys in a location on your computer (client). It can help you to avoid typing the password everytime.
* Here's the step for how to set up:
 ```
 # on client (your computer)
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key
(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
Enter passphrase (empty for no passphrase):
# on client (your computer)
 ```
 * Then you will see the following image to show you save successfully
 * <img width="723" alt="iMAGE STEP5" src="https://user-images.githubusercontent.com/103226676/162672582-7ad9bc1c-5dce-4667-80bc-5bd4d53b7971.png">
 * To use the key you saved, you should do the following code
 ```
 $ ssh cs15lsp22zz@ieng6.ucsd.edu
<Enter Password>
# now on server
$ mkdir .ssh
$ <logout>
# back on client
$ scp /Users/<user-name>/.ssh/id_rsa.pub
cs15lsp22zz@
ieng6.ucsd.edu:~/.ssh/authorized_keys
  ```
 
  
 **Optimiazing Remote running**
 * you can use the up arrow to recall the command you have run
 * or use semicolon to give mutiple command in one time 
 * or you can command in quote at the end of the directoey to run dricectly run it.
 * this is the exapmle to run with up arrow key
 * <img width="356" alt="1649657358(1)" src="https://user-images.githubusercontent.com/103226676/162675218-3f7f6e0c-7aa7-4afb-93a8-91dc13540b4a.png">

 
