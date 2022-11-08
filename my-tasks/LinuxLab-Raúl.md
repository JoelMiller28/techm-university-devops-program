# Git Lab #

## Part 1. Learning SSH ##

1. Tell us a brief history about SSH and why I should learn SSH. 

        This is a program that allows users to execute different commands on the remote machine, be able to access a different computer through the use of the network and move files between two machines. Likewise, this takes care of communications and security authentication.

        You must learn from such a system, because it helps to facilitate secure communications between systems using a client/server architecture, which allows those who use it to connect to a host remotely, also serving as a replacement for rsh and rcp.

2. Document the steps needed to configure an SSH server.



3. Copy one of the files from the previous practice to one of your coworkers, document all the steps and paste screenshots as proofs.



Customize the ssh dir using the configuration file at /etc/ssh/sshd_config and apply the following requirements:

Change the default SSH port Disable access to root user through ssh Create a group to enhance ssh security using the AllowGroups flag and enable ssh access for a new user called letmein, document the process Create an entry banner that displays the text "Welcome stranger to DigitalOnUs" everytime a user ssh into your VM

Config your own ssh using $USER/.ssh/config and make sure when you type server01 it connects to your coworker machine Document how to create an ssh key and how to copy the key into another server




## Part 2. Users and groups ##

Describe the process to:

1. Create a user in Linux 

        In order to create a new usser, you will have to enter the "useradd" command to the system, adding the needed requiremints to be able to work with it. 
        
        There is also another way to do this process:
        
        - Log in to the server with the access data of the root user.
        - Enter the following command: localhost: ~ # useradd USER_NAME. ...
        - To set the password for the new user, enter the following command: [root@localhost ~]# passwd USER_NAME
        - Finally, the password is entered and repeated in order to confirm it

2. Delete a user in Linux 

        For this process, you will simply have to use the "userdel" command on the user in question that you want to delete from the system.

3. Modify a user in Linux 

        To be able to modify users in Linux, you will have to use the "usermod" command, allowing you to make changes, delete things, modify groups and change account attributes, etc.

4. Change user password

        For this you will have to log in, then enter the "passwd" command along with the user name and change the password to the one you want; it is higly recommended to enter a secure password.

5. Describe the different methods to list users in Linux (/etc/passwd, id, w, who, finger)

        In order to display the list of users within Linux, we will have to use the "cat" and "more" commands, but if we want to see the groups to which they belong, we will have to use the command "groups".

6. Create a group in Linux called dou-devops

       In order to create a new user group, one of the following commands will have to be entered: $sudo groupadd groupName or $sudo addgroup groupName. Later you will have to enter the code "groupadd" so that it can be added to the system and modify its name.

7. Add the users dou-YOUR_NAME to the previous group

        In order to add the name, you will have to open the terminal and type ""sudo usermod -c «Your Full True Name» -l New_User_Name Old_User_Name"".

        For example: sudo usermod -c “Raúl Reyes Mont” -l raúl rem

8. Delete the user dou-YOUR_NAME users from the dou-devops group

        However, if you want to delete the username, you will have to use the "userdel username" command in order to remove the configuration seen in the previous point.

9. Describe the different methods to consult groups in Linux

        In order to see the groups that exist within the system, you only have to open the "/etc /group" file, where each line will show the data for a certain group.

10. How can you delete groups in Linux?

        In order to remove it, type "groupdel" along with the group name, this will remove the group entry from /etc/group and /etc/gshadow

11. Tell us the different method to use root privileges

        In order to carry out this operation, you will have to follow the steps shown below:

        1. Click on the lower left corner of the icon, that is, on the start button.
        2. Click on the "Terminal" menu item to open the terminal.
        3. Put the command: "% sudo su –"
        4. Press "Enter". This will turn the terminal prompt into #.
        5. I already have root privileges for each of the operations in the terminal window.


## Part 3. Learning the Linux structure for the directories ##

Follow along the directory workshop and explain in your own words the purpose of each directory:

        Root: This directory is the base for what is known as "the directory tree", it is in this place where the system directories are located.

        Bin: It is a static directory where the binaries that are used to perform basic functions at the user level are stored.

        Boot: It is the one that has the data that is used to initialize the system, such as kernel.

        Dev: It has all the special device files for hardware devices.

        Etc: With this, the configuration files are saved at the component level of the operating system and the programs that are in it.

        Home: This is the standard user directory, used to store user files like photos, documents, templates, etc.

        Lib: The necessary libraries are found so that the binaries of the "bin" directories can be executed correctly.

        Opt: Provides a space where an area can be stored to store all the software packages of a static application.

        Proc: This directory has files that represent the current state of the kernel, allowing users to look at the kernel view of the system.

        Srv: It is the one used to save data and directories used by certain servers installed on the computer.

        Sys: This directory has virtual files that provide kernel data in relation to operating system events.

        Tmp: It is used so that files can be stored temporarily.

        Usr: This saves commonly used programs for general users.
