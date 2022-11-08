# Git Quest #

## Questionary ##

1. What do you mean by Linux? Explain its features.

        Linux is an operating system that is characterized by being free to use, it has an independent code, it is multitasking and multiuser at the same time, its security is quite remarkable and the software is very stable.

2. What are basic elements or components of Linux?

        Some of these components that are part of the operating system are the following: Daemons, Bootloader, the Init System, graphic server, desktop, applications and the Kernel

3. Describe the different types of processes (daemons, zombies, parent, child, etc.)

        daemons: This is a type of program that runs in the background, instead of being controlled directly by users.

        zombies: This is a process which has already completed its execution, however it still has an entry in the process table.

        orphan: These are the opposite of the above, where the parent process ends before its child processes.

        child: This process is created by a parent process within an operating system using a fork system call in order to do it.

        parent: This process is relacionated with the child process, which work together with its respective PIDs

4. How can you list the different kind of processes?

One way in which the processes can be differentiated from each other would be as follows:

    - running (R) : Processes that are being executed.
    - sleeping (S) : Processes that are waiting their turn to be executed.
    - stopped (D) : Processes that are waiting for some input or output operation to be finished.

5. How do you kill a process gracefully? Describe all the steps

        You can kill a process by using its PID, by using its name (or just a part of it), or by selecting the window with the mouse

6. How do you kill a process in the least graceful way? Describe all the steps

        First, the "pgrep pwsh" command is used so that the PID of the pwsh process, used in the kill command, can be determined. Afterwards, kill -s TERM 22687 is used to terminate the pwsh process correctly. And finally, the ps or pgrep commands are used to verify that the PID is no longer listed.

7. How can you check if a daemon is enabled?

In order to check if daemon is enabled, you just have to text this command in the panel:

    $ systemctl status nginx.service
    ## ssh server status ##
    $ systemctl status sshd.service
    ## Lighttpd web server status ##
    $ systemctl status lighttpd.daemon

Then it will show you the results and it will say daemon is running in the background, or else you will have to find the main cause of the interruption 

8. Tell us what is a soft link and a hard link

        Soft links act as a chain that is responsible for producing paths for different directories and files within the computer system. 
        
        While hard links refer to more than one file sharing the same inode, being a copy of the rest of the linked files.

9. What is a pipe and how does it work?

        The pipeline command is one that allows the output of one command to be sent to another, and may be able to redirect the input, output or error from one process to another in order to be processed.

10. What is an RPM package?

        This is the tool that is responsible for managing the packages considered for GNU/Linux, thus being able to update, install and verify programs.

11. What is a dependency in Linux?

        This is how all the necessary packages are called so that a different package can be installed and also executed.

12. What is a repository in Linux?

        Those are the file servers that are within a certain distribution, being the dependency managers the ones that connect to the servers when they need to install an application and its respective dependencies.

13. What is BASH?

        This is the name given to the parameters that are used for the configuration and administration of the system, as well as the set of key combinations to perform certain tasks.

14. What is CLI and GUI?

        In short, CLI is the line interface that allows you to interact with the system through the use of multiple commands, while GUI ensures that users can interact with the system using graphics, such as icons or images.

## Commands ##

Explain and give an example of the following commands:

ls: It is responsible for enumerating and listing the content of the directory that is desired, such as files and nested directories.

cp: Command used so that different files can be copied from the current directory to move them to a different directory.

mv: It is used so that directories found in the file system can be renamed or moved.

rm: This deletes each of the documents that are indicated within the directory line, however you have to be very careful with this, because it is difficult to recover a deleted file.

du: This command displays disk usage recursively across existing directories and within a set of files.

df: Thanks to the use of this command, the space on the disk used by the file system is shown.

pwd: It is the one that is responsible for locating the path of the working directory in which the user is currently located.

mkdir: This allows users to create directories, helping to create multiple directories at once, as well as generating permissions for directories.

cat: It takes care of concatenating and reading files, as well as writing and combining the files to standard output.

more: It is used so that the content of a file can be seen and observed by pages, but without the possibility of modifying what is in i. 

less: In this you can see page by page the content of the file that is taken as an argument.

cd: Thanks to the use of this command, you may be able to navigate through the directories within the system, performing some functions such as changing the current directory to a new one.

touch: It is used so that any new type of file can be generated, being useful for creating files within the server.

clear: As its name indicates, it is used to erase everything that is on the screen.

tail: This command is used to display the last lines of a specific file.

head: It is the opposite of the previous command, now showing the first lines of text inside the file.

history: It is very useful to know the last commands that have been executed within a server.

eject: Allows removable media drives to be ejected from the hardware using software commands.

uname: It is used to display the data of the operating system, such as its name or version.

blkid: It is responsible for teaching the type of block device file system, as well as its attributes.

lspci: This system is responsible for displaying the lists with data about the devices and buses that are in the system.

file: This command is responsible for doing a series of tests to define the format and type of a file.

date: When this command is used, the system date and time are shown to the user, giving the opportunity to modify it.

clock: It is used to define the time it takes for a specific operation to be executed.

uptime: Provides information about the current time, users online, system uptime, and system load.

last: This shows a list of users who have logged in, the system where they did so, and their respective date and time.

man: With this command it is possible to know the use of Linux commands, showing basic information such as the name, its description, the options it has, versions, exit status, return values, etc.

last login: This command is used so that the last login times for the different users who have previously accessed can be found.

poweroff: It works the same as the "shutdown" command, allowing us to turn off the system, but it doesn´t give us the possibility to declare additional options such as messages.

reboot: This takes care of rebooting Linux as standard

exit: Takes care of getting the user out of super user mode to admin