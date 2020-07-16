# devops-doc

DevOps Documentation

##Linux commands
##Shows various Beginners level Linux Commands.

###ls commands

#####ls
ls with no option list files and directories in bare format 

#####ls -l
 shows file or directory, size, modified date and time, 
 file or folder name and owner of file and its permission.
 
 #####ls -a
 
 shows the file directory including the hiiden files.
 
 #####ls -lh 
 Shows the file sizes in the human readable formats.
 
 #####ls -F
 puts '/' in front of those those which are directories.
 
 #####ls -r
 lists the files in reverse order.
 
 #####ls -R
 used to recursively list the sub-directories of each folder,sub-folder,etc
 
 #####ls -ltr
 Shows the latest modified files at top
 
 #####ls -ls
 Displays the file sizes in descending orders.
 
 #####ls -i
 Displays the inode no. of the files.
 
 #####ls --version 
 used to check the version of ls.
 
 #####ls --help
 used to display the help page of ls commands.
 
 #####ls -l /tmp
 Used to list the temporary files in the directory.
 
 ##### ls -n
 used to display the GID and UID of the files.
 
 ###lsblk
 The first column lists device names, followed by corresponding major and minor device numbers, whether or not the device is removable (1 in case it is), size of the device, whether or not the device is read only, type of device (disk, partition, etc), and finally the device's mount point (if available).
 
 #####lsblk -a 
 Displays the empty devices only.
 
 #####lsblk -b
 lists the size of each disk in the form of bytes.
 
 #####lsblk -z
 prints zone model for each device.
 
 #####lsblk -d 
 skip the entries of slaves in listing.
 
 #####lsblk -i
 use ascii characters for tree formatting.
 
 #####lsblk -m 
 displays info about device owner,group and mode.
 
 #####lsblk -o col1,col2
 displays only the specified columns at a time.
 
 ###md5sum command
 #####md5sum/home/mandeep/test/test.cpp
 It is a very important command used to verify whether the person who created the file has not made any change to it before giving it to the other person.
 It generates 128-bit checksum .md5 file.
 
 md5sum /home/mandeep/test/test.cpp > checkmd5.md5
 
 md5sum -c checkmd5.md5
 
 /home/mandeep/test/test.cpp: OK
 
 After changing the contents of file checkmd5.md5, the output will be :
 
 
 /home/mandeep/test/test.cpp: FAILED
 md5sum: WARNING: 1 computed checksum did NOT match
 
 ###uname command
 
 #####uname
 Prints Kernel name, network node hostname, kernel release date, kernel version, machine hardware name, hardware platform, operating system.
 
 #####uname -s
 prints the kernel name
 
 #####uname -n
 prints the hostname of the network node(current computer).
 
 #####uname -r
 prints the kernel release date.
 
 #####uname -v
 prints the version of the current kernel.
 
 #####uname -m
 prints the machine hardware name.
 
 #####uname -p
 It prints the type of the processor.
 
 #####uname -i
 It prints the platform of the hardware.
 
 #####uname -o
 It prints the name of the operating system.
 
 ###history commands
 
 #####history
 Gives you a complete list of previously executed programs.
 
 
 #####export HISTTIMEFORMAT='%F %T  '
 displays the time and date of the history commands.
 
 #####export HISTCONTROL=ignoredups
 **Ignore Duplicate** commands in history.
 
 #####history -c
 **Clearing** all the entries from the bash history.
 
 #####history | grep *command_name*
 Used to search for a specific command in history.
 
 #####*PRESS CTRL+R* source .bash_profile
 Search for Prevoiusly Executed Commands
 
 #####!*line_no*
 Display the command runned at a specific line number.
 
 ###Sudo Commands
 
 #####sudo -v
 The -V (version) option causes sudo to print the version number and exit.
 
 #####sudo -l 
 Prints the commands allowed (and forbidden) for the current host/user.
 
 #####sudo -L
 List out the parameters that may be set in a Defaults line along with a short description for each. This option is useful in conjunction with grep.
 
 #####sudo -h
 Displays a Guide for sudo commands.
 
 #####sudo -v
 Update the user's timestamp, prompting for the user's password if necessary.
 
 #####sudo -k
 Used to revoke a User's sudo permission.
 
 #####sudo -K
 Used to removes the user's timestamp entirely.
 
 #####sudo -b
 Removes the user's timestamp entirely.
 
 #####sudo -p
 The -p (prompt) option allows you to override the default password prompt and use a custom one. The following percent ('%') escapes are supported:
 
 %u is expanded to the invoking user's login name;
 
 %U is expanded to the login name of the user the command will be run as (which defaults to root);
 
 %h is expanded to the local hostname without the domain name;
 
 %H is expanded to the local hostname including the domain name (only if the machine's hostname is fully qualified or the "fqdn" sudoers option is set);
 
 %% (two consecutive % characters) are collapsed into a single % character. 
 
 #####sudo -c
 Run the specified command with resources limited by the specified login class.
 
 #####sudo -a
 Used to specify authentication type to validate a user.
 
 #####sudo -u
 Used to run a specific command as a user other than root.
 
 #####sudo -s
 Runs the Shell as specified by the SHELL Environment variable else as specified in the passwd file.
 
 #####sudo -H
 Sets the Home Environment variable to the home directory of the target user(root by default)
 
 #####sudo -r
 The -r (role) option causes the new (SELinux) security context to have the role specified by ROLE.
 
 #####sudo -S
 Causes sudo to read the password from standard input instead of the terminal device.
 
 #####sudo --
 indicates that sudo should stop processing command line arguments.
 
 ###mkdir commands
 
 #####mkdir *directory_name*
 Used to create a directory.
 
 ###touch commands
 
 ####touch *file_name*
 Creates a file without having content in it.
 
 ####touch *file_name1 file_name2*
 Create multiple files at a time.
 
 #####touch -a *file_name*
 Changes the access time of a file.
 
 #####touch -c *file_name*
 Check whether a file is created or not. If not created then don’t create it. This command avoids creating files.
 
 #####touch -c-d *file_name*
 Used to update access time and modification time.
 
 #####touch -m *file_name*
 Used to update access time only.
 
 #####touch -r *second_file_name* *first_file_name*
 This command is used to use the timestamp of another file
 
 #####touch -t *YYMMDDHHMM* *fileName*
 Used to create a file using a specified time.
 
 ###chmod commands
 
 #####chmod u=r *file_name*
 Owner can only read the file.
 
 #####chmod u=rw *file_name*
 Owner cand read as well as write the file.
 
 ###chown commands
 
 #####chown *owner_name file_name*
 Used To change the ownership of the file.
 
 #####chown -c *file_name*
 Reports when a file change is made.
 
 #####chown -v *file_name*
 Used to show the verbose information for every file processed.

 #####chown :*group_name* *file_name*
 Change group ownership.
 
 #####chown *owner_name*:*group_name* *file_name*
 Change owner as well as group.
 
 #####chown --from=*owner_name1* *owner_name2* *file_name*
 Change the owner from particular ownership only.
 
 #####chown --from=:*group_name* *owner_name* *file_name*
 Change Group for a particular group.
 
 #####chown --reference=*file_name1* *file_name2*
 Copy ownership of one file to another.
 
 #####chown master:*group_name* *file_name2* *file_name3*
 Change ownership of multiple files.
 
 ###apt commands
 
 #####apt update
 Used when we want to download package information from all configured sources.
 
 #####apt upgrade
 Used to install all available upgrades of all packages currently installed in the system.
 
 #####apt full-upgrade
 Used to upgrade the system as a whole, if the removal of already installed packages is required, then it will remove them.
 
 #####apt install *package_name*
 Used to install one or more packages.
 
 #####apt remove
 Used to remove or delete installed packages.
 
 #####apt purge
 Similar to remove. Specially removes configuration files of the removed packages.
 
 #####apt autoremove
 Used when the user wants to remove the packages that were installed as dependencies.
 
 #####apt search 
 Search for a Package.
 
 #####apt show
 Used to show the information related to packages. like dependencies,installation size,sources.
 
 #####apt list
 Used to display the packages that quality a certain criteria.
 
 #####apt edit-sorces
 Allows editing sources.list file.
 
 #####apt --help
 Display a guide for apt command.
 
 #####apt --version
 Displays the installed apt version.
 
 ###tar commands
 
 #####tar cvf *file_name.tar* **extension_type*
 Creates a tar file of all files of given extension.
 
 #####tar xvf *file_name*.tar
 Extracts files from archives.
 
 #####tar cvzf *file_name*.tar.gz **extension_type*
 Creates a tar file with .gz compression.
 
 #####tar xvzf *file_name*.tar.gz
 Extracts files from tar.gz archive.
 
 #####tar cvfj *file_name*.tar.tbz *file_name*
 Compresses and creates lightweight archive than gzip.
 
 #####tar xvfj *file_name*.tar
 Untar the file.
 
 #####tar tvf file.tar
 View archive
 
 #####tar xvf *file_name*.tar "file_name" *"file_name"* 
      or 
 #####tar zxvf *file_name*.tar.gz "file_name" *"file_name"*
      or 
 #####tar jxvf *file_name*.tar.tbz "file_name" *"file_name"*
 Untar multiple tar files.
 
 #####tar czf *file_name*.tar/tar.gz/tar.tbz | wc -c
 Display size of existing tar files in KB.
 
 ###cal command
 
 #####cal
 Display Calender of current month.
 
 #####cal *DD YYYY*
 Display calender of specified month.
 
 #####cal *YYYY*
 Display Calender of all months of the specified year.
 
 #####cal -3
 Display Calendar of previous, current and next month.
 
 ###date Commands
 
 #####date 
 Shows current date.
 
 #####date --set=*'DD month_name Year HH:MM'*
 Sets the given date.
 
 ###cat commands
 
 #####cat *file_name*
 View a single file.
  
 #####cat *file_name1* *file_name2*
 View two or more files.
 
 #####cat -n *file_name*
 View contents of file with line numbers.
 
 #####cat >*file_name*
 Create file.
 
 #####cat [filename-whose-contents-is-to-be-copied] > [destination-filename]
 Copy contents of one file to another.
 
 #####cat -s *file_name*
append the contents of one file to the end of another file. Eliminate all empty lines in file.
 
 #####cat *file_name1*>>*file_name2*
 Append the contents of one file to the end of another file.
 
 #####tac *file_name*
 Display Contents of file in reverse order.
 
 #####cat -A *file_name*
 Uses -v,-E,-T option together.
 
 ###cp command
 
 #####cp *SOURCE_PATH* *file_name* *DEST_PATH*
 Copies files from Source to destination.
 
 ###mv command
 
 #####mv *SOURCE_PATH* *file_name* *DEST_PATH*
 Moves files from Source to destination.
 
 ###pwd command
 
 #####pwd
 Prints working Directory.
 
 ###cd commands
 
 #####cd *file_name*/*PATH*
 Access the following file present at a PATH.
 
 ##Shows various Intermediate level Commands
 
 ###find commands
 
 #####find ./*directory_name* -name '*file_name*'
 Search for the given file in the specified directory.
 
 #####find ./*directory_name* -name '**extension_type*'
 Searches for a specified extension of a file.
 
 #####find ./*directory_name* -name '*file_name*' -exec rm -i {} \;
 Find and delete a file with confirmation.
 
 #####find ./*directory_name* -empty
 Find all empty folders and files in the mentioned directory.
 
 #####find ./*directory_name* -perm *absolute_code*
 Absolute code can be a combination of 4-Read, 2-Write, 1-Execute, 0-no permission
 Command is used to display files which satisfy the Access specified in *absolude code*
 
 #####find ./ -type f -name "*.*extension_type*" -exec grep '*Search Keyword*'  {} \;
 Searches for a Specific keyword in file and prints the lines where the keyword exists.
 
 ###grep commands
 
 #####grep -i "*Search_keyword*" *file_name.txt*
 Performs a Case insensitive search for the keyword in the specified file
 
 #####grep -c "*Search_keyword*" *file_name.txt*
 Displays the number of lines which has the *Search_keyword*
 
 #####grep -l "*Search_keyword*" *
 Display the file names that matches the *Search_keyword*
 
 #####grep -w "*Search_keyword*" *file_name.txt*
 Display the files having the *Search_keyword* as a Substring.
 
 #####grep -o "*Search_keyword*" *file_name.txt*
 Displays only the matched pattern.
 
 #####grep -n "*Search_keyword*" *file_name.txt*
 Shows the line number of file with the line Matched.
 
 #####grep -v "*Search_keyword*" *file_name.txt*
 Display the lines that are not matched with the specified *Search_Keyword*.
 
 #####grep "*^Search_keyword*" *file_name.txt*
 Displays the lines starting with *Search_keyword*
 
 #####grep –e "*Search_keyword1*" –e "*Search_keyword2*" –e "*Search_keyword3*" *file_name.txt*
 Accepts multiple *Search_keyword* in the file at a time.
 
 #####grep -f "*Search_file.txt*" *file_name.txt*
 Takes patterns from file, one per line.
 
 ###man commands
 
 #####```man <command_name>```
 Manual pages of the command are simply returned.
 
 #####```man <section_num> <command_name>```
 Used to display only a specific section of a manual.
 
 #####```man -f <command_name>```
 Lists the section in which the *command_name* exists.
 
 #####```man -a <command_name>```
 Display all the available manual pages of the specified *command_name* in succession.

 #####```man -k <command_name>```
 Searches the given command as a regular expression in all the manuals and it returns the manual pages with the section number in which it is found.
 
 #####```man -w <command_name>```
 Returns the location in which the manual page of a given command is present.
 
 #####```man -I <command_name>```
 Considers the command as case sensitive.
 
 ###ps commands
 
 #####```ps```
 Shows the processes for the current shell.
 
 #####```ps -A```
 View all the running processes.
 
 #####```ps -a```
 Views processes not associated with the terminal and session leaders.
 
 #####```ps -d```
 View all the processes except the session leaders.
 
 #####```ps -a -N```
 View only the processes related to the session leader and process not associated with the terminal.
 -N is just used to negate a command.
 
 #####```ps -T```
 View process associated with terminal.
 
 #####```ps -r```
 View all running processes.
 
 #####```ps -x```
 View all processes owned by you.
 
 ###kill commands
 
 #####```kill -l```
 Display all the available signals.
 
 #####```kill pid```
 kill a process using it's Process ID.
 
 #####```kill {-signal | -s signal} pid``` 
 Send signal to Process.
 
 #####```kill {-l | --list[=signal] | -L | --table}``` 
 Used to list available signals in a table format.
 
 ###whereis commands
 ####```whereis <directory_name> -f <file_name>```
 #####-b
 Search only for binaries.
 
 #####-m
 Search for manual sections.
 
 #####-s
 Search only for sources.
 
 #####-u
 Search for unusual entries.
 
 #####-B
 Change or otherwise limit the places where whereis searches for binaries.
 
 #####-M
 Change or otherwise limit the places where whereis searches for manual sections.
 
 #####-S
 Change or otherwise limit the places where whereis searches for sources.
 
 #####-f
 Terminate the last directory list and signals the start of file names, and must be used when any of the -B, -M, or -S options are used.
 
 Eg-
 1.```whereis gcc```
   List the directories where the gcc source files, documentation, and binaries are stored.
 2.```whereis``` -u -M /usr/man/man1 -S /usr/src -f *
   Find all files in the current directory that are not documented in /usr/man/man1, whose source resides in /usr/src.
 
 ###service commands
 
 #####```service <SCRIPT-Name> stop```
 Used to stop a service.
 
 #####```service <SCRIPT-Name> start```
 Used to start a service.
 
 #####```service <SCRIPT-Name> status```
 Used to know the status of a service.
 
 #####```service <SCRIPT-Name> restart```
 Used to start a service again.
 
 ###df commands
 
 #####```df *OPTION* *FILE*```
 Used to display total space and available space.
 
 #####options for df commands
 
 -a, –all : includes pseudo, duplicate and inaccessible file systems.
 
 -B, –block-size=SIZE : scales sizes by SIZE before printing them.
                        It will also need a parameter of size to be mentioned.
                        
 -h, –human-readable : print sizes in power of 1024
                       Eg- ```df -B 1024``` 
                       gives output like-
                       1023 MB
                       
 -H, –si: print sizes in power of 1000
          gives output like-
          1.1 GB
          
 -i, –inodes : list inode information instead of block usage
 
 -l, –local : limit listing to local file systems
              Eg- converts data from human-readable form into Kilo-bytes.
 
 -P, –portability : use POSIX output format.
                    
 
 –sync : invoke sync before getting usage info
 
 –total : elide all entries insignificant to available space, and produce grand total
 
 -t, –type=TYPE : limit listing to file systems of type TYPE
 
 -T, –print-type : print file system type 
 
 ###du commands
 
 #####```du <directory_name>```
 
 #####Options for du
 -0, –null : end each output line with NULL
 
 -a, –all : write count of all files, not just directories
 
 –apparent-size : print apparent sizes, rather than disk usage.
 
 -B, –block-size=SIZE : scale sizes to SIZE before printing on console
 
 -c, –total : produce grand total
 
 -d, –max-depth=N : print total for directory only if it is N or fewer levels below command line argument
 
 -h, –human-readable : print sizes in human readable format
 
 -S, -separate-dirs : for directories, don’t include size of subdirectories
 
 -s, –summarize : display only total for each directory
 
 –time : show time of of last modification of any file or directory. This command is much equivalent to ```ls -l``` command Just the difference is --time will not show the Access Specifier. i.e. -rwx/-rw,etc.
 
 –exclude=PATTERN : exclude files that match PATTERN 
 
 ###rm commands
 
 #####```rm -i <file_name>```
 Asks the user for confirmation before deleting each file.
 
 #####```rm -f <file_name>```
 Prompts for file deletion if a file is write protected.
 
 #####```rm -r <file_name>```
 Performs a tree-walk and will delete all the files and sub-directories recursively of the parent directory.
 
 #####```rm --version```
 Specified the version of rm
 
 #####```rm -- -<file_name>```
 Remove a file whose name begins with a dash (“-“).
 
 ###echo commands
 
 #####```echo "String"```
 Prints a simple String.
 
 #####Options in Echo command
 -e:Here enables the interpretation of backslash escapes. \n can be used for new line, \c can be used for eliminating the code after \c. \t acb be used for creating tab spaces in string.\r can be used
 
 Example:

 
 ```echo "Shubham \bIs \bExcellent"```
 
 Output
 ```
 ShubhamIsExcellent
 ```
 
 ###passwd commands
 
 #####passwd <options> <username> 
 -d, –delete: This option deletes the user password and makes the account password-less.
 
 -e, –expire: This option immediately expires the account password and forces the user to change password on their next login. 
 
 -h, –help: Display help related to the passwd command.

 -i, –inactive INACTIVE_DAYS: This option is followed by an integer, INACTIVE_DAYS, which is the number of days after the password expires that the account will be deactivated. 

 -k, –keep-tokens: This option is used when you only want to change the password if it is expired. It keeps the authentication tokens for the authentication if the password is not yet expired, even if you requested to change it. Note that if the expiry period for a user is set to 99999, then this option will not keep tokens and the password will be changed.
 
 -l, –lock: Lock the password of user. This appends the encrypted password of the user with a character ‘!’, and thus making it unable to match with any of input password combinations. This does not disable the account but prevents the user from logging in using a password. Though other authentication methods like ssh keys can be used to login to the account.
 
 -n, –mindays MIN_DAYS: Change the minimum number of days between password changes to MIN_DAYS so that the user can’t change the password for MIN_DAYS.
 
 -q, –quiet: This option is used for quiet mode. While using this option to change a password, the message “Changing password for $user.”, which usually gets printed before changing a password, does not get echoed. 

 -r, –repository REPO: This option is used to change password for repository named “REPO”.
 
 -R, –root CHROOT_DIR: Apply changes in the CHROOT_DIR directory and use the configuration files from the CHROOT_DIR directory. This basically changes the root directory for the passwd process for once, and since CHROOT_DIR is a sub-directory of the root, it can not access the configuration files outside the CHROOT_DIR.
 
 -S, –status: Shows the password status (7 fields) of user.
 
 -u, –unlock: Unlock the password of an account.
 
 -w, –warndays WARN_DAYS: This option is used to change the number of days before the password is to expire, to display the warning for expiring password.
 
 -x, –maxdays MAX_DAYS Set the maximum number of days for which the password remains valid. After MAX_DAYS, the password will expire and the user will be forced to change password.
 
 
 ###cmp commands

```cmp <option> <file1> <file2>```

#####options for cmp commands
-b(print-bytes) : If you want cmp displays the differing bytes in the output when used with -b option.

-i [bytes-to-be-skipped] : This option when used with cmp command helps to skip a particular number of initial bytes from both the files and then after skipping it compares the files. This can be done by specifying the number of bytes as argument to the -i command line option.

-l option : This option makes the cmp command print byte position and byte value for all differing bytes.

-s option : This allows you to suppress the output normally produced by cmp command i.e it compares two files without writing any messages. This gives an exit value of 0 if the files are identical, a value of 1 if different, or a value of 2 if an error message occurs.

-n [number of bytes to be compared] option :This option allows you to limit the number of bytes you want to compare ,like if there is only need to compare at most 25 or 50 bytes.

 – -v option : This gives the output information and exits.

 – -help option : This displays a help message and exits.
 
 ###wget commands
 
 #####```wget <download link>```
 Downloads the file given at the link.
 
 #####```wget -o <file_name required by user> <download_link>```
 Downloads the file with specified name by user.
 
 #####```wget <http_link> <ftp_link>```
 Downloads files from http and ftp link at once.
 
 #####```wget -i <file_path>`` 
 Reads URL from a file.
 
 #####```wget -c <download_link>```
 Resumes an incomplete download.
 
 #####```wget -b <download_link>```
 Downloads the file in background.
 
 #####```wget --limit-rate=<kbps> <download_link> ```
 Limits the download speed of the specified file.
 
 #####```wget --http-user=<Username> --http-password=<password> <download_link>```
 Used to download password restricted http in which ```--http-user``` and ```--http-password``` will be defined by the URL and specified in the command by the user.
 
 #####```wget --ftp-user=<Username> --ftp-password=<password> <download_link>```
 Used to download password restricted ftp in which ```--http-user``` and ```--http-password``` will be defined by the URL and specified in the command by the user.

 #####```wget --version```
 Display version of wget.
 
 #####```wget --help```
 Display help for wget
 
 ###gcc/g++ commands
 ```gcc -c|-S|-E -std=standard```
 
 ####Options for gcc commands
 
 -o opt: This will compile the source.c file but instead of giving default name hence executed using ./opt, it will give output file as opt. -o is for output file option. 
         Example: ```gcc program.c -o opt```
 
 -Werror: Displays warnings as well for a program.
 
 -Wall: Displays errors as well as warnings for the program.
 
 -ggdb3: Gives permission to debug the program using GNU Debugger.
 
 -lm: Used to link ```math.h``` library to our program/Soure Code.
 
 -std=c11: Used to apply c11 standard for compiling the source code.
 
 -c: Compile the program and give the object file as output, which is used to make libraries.  
 
 -v: Used for the verbose purpose.
 
 ###ifconfig commands
 
 #####```ifconfig```
 Displays all the active interfaces in detail.
 
 #####```ifconfig -a```
 Displays all active as well as inactive interfaces on server.
 
 #####```ifconfig <name_of_interface>```
 Used to display a specific interface.
 
 #####```ifconfig <name_of_interface> up```
 Used to activate an interface.
 
 #####```ifconfig <name_of_interface> down```
 Used to deactivate an interface.
 
 #####```ifconfig <name_of_interface> <IP_Address>```
 Assign IP address to a specified interface.
 
 #####```ifconfig <name_of_interface> netmask <Network_mask>```
 Assign a Network Mask to a specified interface.
 
 #####```ifconfig <name_of_interface> broadcast <Broadcast_address>```  
 Assign a Broadcast address to the specified interface.
 
 #####```ifconfig <name_of_interface> <IP_Address> netmask <Network_mask> broadcast <Broadcast_address>```
 Assign IP,Netmask and Broadcast to an interface.
 
 #####```ifconfig <name_of_interface> mtu <Max_Transmission_Unit>```
 Set the MTU for the interface specified by the user.
 
 ####Other Networking Utilities
 tcmpdump- It is a command-line packet capture and analyzer tool for monitoring network traffic.
 
 Wireshark- An open source network protocol analyzer that is used to troubleshoot network related issues.
 
 Munin- A Web based network and system monitoring application that is used to display results in graphs using rrdtool.
 
 Cacti- Complete web based monitoring and graphing application for network monitoring. 

 ###netstat commands
 
 #####```netstat -a|more```
 Show Listening and non-listening Sockets.
 
 #####```netstat -at```
 List all TCP ports.
 
 #####```netstat -au```
 List all UDP ports.
 
 #####```netstat -l```
 List all listening ports.
 
 #####```netstat -lt```
 List all listening TCP ports.
 
 #####```netstat -lu```
 List all listening UDP ports.
 
 #####```netstat -lx```
 List only the listening UNIX ports.
 
 #####```netstat -s```
 List Statistics for all ports.
 
 #####```netstat -st(TCP)```
 List Statistics for TCP ports. 

 #####```netstat -su(UDP)```
 List Statistics for UDP ports.

 #####```netstat -pt```
 Display PID and program names.
 
 #####```netstat -c```
 Prints Netstat Information continuously.
 
 #####```netstat -verbose```
 Gets the non-supportive address families in the system.
 
 #####```netstat -r```
 Get the Kernel routing information.
 
 #####```netstat -ap | grep <protocol_name>```
 Get the port on which program is running.

#####```netstat -an | grep :<port_no> ```
Get the process which is using the specified port.

#####```netstat -i```
List of Network interfaces.

#####```netstat -ie```
Dipslay interfaces in detail.

###nslookup commands

#####```nslookup <domain>```
Displays 'A' record of specified domain.

#####```nslookup <Address>
Display reverse domain lookup

#####```nslookup <name>```
Display Specific domain lookup.

#####```nslookup -query=mx <URL>```
To Query mail exchange record.

#####```nslookup -query=ns <URL>```
To query Name Server Record.

#####```nslookup -type=soa <URL>```
To query Start Of Authority Record.

#####```nslookup -query=any <domain>```
To query all Available DNS Records.

#####```nslookup -debug <Domain>```
Enable debug mode.

###dig commands 

#####```dig <domain>```
Query Domain “A” Record.

#####```dig <domain> +short```
Query Domain “A” Record with +short.

#####```dig <domain> MX```
Querying MX Record for Domain.

#####```dig <domain> SOA```
Querying SOA Record for Domain.

#####```dig <domain> TTL```
Querying TTL Record for Domain.

#####```dig <domain> +nocomments +noquestion +noauthority +noadditional +nostats```
Querying only answer section.

#####```dig <domain> ANY +noall +answer```
Querying ALL DNS Records Types.

#####```dig -x <Address> +short```
DNS Reverse lookup.

#####```dig <Domain> mx +noall +answer redhat.com ns +noall +answer```
Querying Multiple DNS Records.

###uptime commands

```uptime -<options>```

#####```uptime -p```
Shows th PC wakeup time on human Readable format.

#####```uptime -s```
Display the time/date since when the system has been running.

#####```uptime -V```
Display Version Information.

#####```uptime -h```
Display help for uptime commands.

###wall commands
```wall <filename>```

#####Options for wall
-n,--nobanner: Suppress banner.


-t,--timeout: Write timeout to terminals in seconds.

-V,--version: Display Version.

-h,--help: Display Help message.

#####mesg commands

#####```mesg y```
Allow other users to send you messages.

#####```mesg n```
Disallow other users to send you messages.

#####```mesg```
Display current status of the terminal.

###talk commands

#####Options in talk command
person: If you wish to talk to someone on your own machine, then person is just the person's login name.  If you wish
        to talk to a user on another host, then person is of the form ‘user@host’ ( or ‘host.user’ or ‘host!user’ or
        ‘host:user’ ).

-x: If you wish to talk to a user who has dot character in username, the -x argument will force ‘user@host’ form
    of the person and talk will take dots as part of user name.

ttyname: If you wish to talk to a user who is logged in more than once, the ttyname argument may be used to indicate
         the appropriate terminal name, where ttyname is of the form ‘ttyXX’ or ‘pts/X’.

###w command

#####options for w command
-h, --no-header: Don't print the header.

-u, --no-current: Ignores the username while figuring out the current process and cpu times. (To see an example of this, switch to   			  the root user with "su" and then run both "w" and "w -u".)

-s, --short: Display abbreviated output (don't print the login time, JCPU or PCPU times).

-f, --from: Toggle printing the from (remote hostname) field. The default as released is for the from field to not be printed, 		    although your system administrator or distribution maintainer may have compiled a version in which the from field is 		    shown by default.

--help: Display a help message, and exit.

-V, --version: Display version information, and exit.

-o, --old-style: Old style output (prints blank space for idle times less than one minute).

user: Show information about the specified the user only.

###rename commands
rename <file_name>

#####Options for remove command

-v,--verbose: Print names of files succesfully renamed.

-n,--no-act: Show what files should have been renamed.

-f,--force: Overwrite existing files.

###top commands

#####```top```
Shows th Ongoing processes.

#####```top -u <process_name>```
Shows th processes related to specified process name.

#####```top -n 1 -b > <file_name.txt>```
Saves the top command result in the file.

#####```top --help```
Display top command help.

#####top -n <repetition_value>
Exit top command after specific repetition.

  



