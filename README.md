# Linux_commands
Useful Linux commands

### File Commands
| Command                 | Result                              |
| :---------------------- | :-----------------------------------|
| ls                      | directory listing |
| ls -al                  | formatted listing with hidden files |
| cd directory            | change directory to directory |
| cd ~                    | change to home directory |
| pwd                     | show current directory path |
| mkdir new_folder        | create directory new_folder |
| rm file_to_delete.txt   | delete file file_to_delete.txt |
| rm -r new_folder        | delete directory new_folder |
| rm -f file_name.txt     | force delete file file_name.txt |
| rm -rf folder_to_delete | force delete folder folder_to_delete |
| cp file1 file2          | copy file1 and name it file2 |
| mv file1 file2          | rename file1 to file2 |
| ln -s file ~/link       | create symbolic link ~/link -> file |
| touch note.txt          | create or update note.txt |
| cat > log.txt           | place standard input into log.txt |
| more log.txt            | output the contents of the file |
| less log.txt            | output the contents of the file |
| head log.txt            | output first 10 lines of the file |
| tail log.txt            | output last 10 lines of the file |
| tail -f log.txt         | output contents of the file as it grows |

### Add Users

| Command                                              | Result                                          |
| :--------------------------------------------------- | :-----------------------------------------------|
| useradd -m username                                  | Create a user name username with home directory |
| useradd -m -p $(openssl passwd -1 password) username | Create user with password password              |
| adduser newuser                                      | Create newuser with on screen prompt            |
| usermod -aG sudo newuser                             | Add newuser to sudo group                       |
| groups newuser                                       | List newuser's group                              |
| deluser newuser sudo                                 | Remove newuser from sudo group                  |
| userdel -r username                                  | Delete username user and user's home directory  |
* -m The user???s home directory will be created if it does not exist.
* -p Create user with password provided.
* username Create this user to the system.

### SSH

| Command                     | Result                              |
| :-------------------------- | :-----------------------------------|
| ssh user@server_ip          | connect to server_ip host as user |
| ssh -p 8888 user@ server_ip | connect to server_ip host as user using port 8888 |
| ssh -D 8889 user@ server_ip | connect to server_ip host as user using bind port 8889 |

### INSTALLATION
| Command      | Result                  |
| :----------- | :-----------------------|
| ./install    | run the install script  |
| make         | ---                     |
| make install | ---                     |

### NETWORK
| Command            | Result                    |
| :----------------- | :------------------------ |
| ping host          | ping host                 |
| whois google.com   | get whois for google.com  |
| dig google.com     | get DNS for google.com    |
| dig -x 192.168.1.1 | reverse lookup host       |
| wget file          | download file             |
| wget -c file       | continue stopped download |
| wget -r url        | recursively download file from URL |

### SYSTEM INFO

| Command            | Result                    |
| :----------------- | :------------------------ |
| date               | show current date/time |
| cal                | show this month calendar |
| uptime             | show the system uptime |
| w                  | display who is online |
| whoami             | display who are you logged in as |
| uname -a           | show kwenal config |
| cat /proc/cpuinfo  | show cpu info |
| cat /proc/meminfo  | show memory information |
| man command        | show manual for command |
| df                 | show disk usage |
| du                 | show directory space usage |
| du -sh             | show directory usage in human readable size unit |
| free               | show memory and swap usage |
| whereis app        | display possible location of the app |
| which app          | display which app will be run by default |

### SEARCH
| Command                 | Result                                |
| :---------------------- | :------------------------------------ |
| grep pattern file.txt   | search for pattern in file.txt        |
| grep -r pattern dir     | search recursively for pattern in dir |
| command \| grep pattern | search the pattern in the output of the command |
| locate file             | find all instances of file |

### PROCESS MANAGEMENT
| Command      | Result                                |
| :----------- | :------------------------------------ |
| ps           | display currently active processes |
| ps aux       | display currently active processes |
| kill pid     | kill process with pid 'pid' |
| killall proc | kill all processes name proc |
| bg           | lists stopped/background jobs, resume stopped job in the background |
| fg           | bring most recent job to foreground |
| fg n         | brings jobs n to foreground |

### FILE PREMISSIONS
chmod octal file - change permission of file<br>

4 - read (r)<br>
2 - write (w)<br>
1 - execute (x)<br>

order: owner/group/world<br>
eg:<br>
chomd 777 - rwx for exeryone<br>
chmod 755 - rw for owner, rx for group and world<br>

### COMPRESSION
| Command                  | Result                                |
| :----------------------- | :------------------------------------ |
| tar cf file.tar file.jpg | tar file.jpg into file.tar |
| tar xf file.tar          | untar into current directory |
| tar tf file.tar          | show contents of archive |
| tar -cvfz ~/Desktop/target.tar.gz folder_to_compress/ | tar and gzip folder_to_compress to target.tar.gz |
| tar xvf target.tar.gz    | unzip and untar target.tar.gz into current directory |

tar flags:<br>
c - create archive<br>
t - table of contents<br>
x - extract<br>
f - specifies filename<br>
z - use zip/gzip<br>
j - bzip2 compression<br>
k - do not overwrite<br>
T - files from file<br>
w - ask for confirmation<br>
v - verbose<br>

### SHORTCUTS
| Command                  | Result                                |
| :----------------------- | :------------------------------------ |
| ctrl+a | Move to the start of the line. |
| ctrl+e | Move to the end of the line. |
| ctrl+c | halt current command |
| ctrl+z | stop current command |
| fg     | resume stopped command in forground |
| bg     | resume stopped command in background |
| ctrl+d | log out of current session |
| ctrl+w | erases one word in current line |
| ctrl+u | erases whole line |
| ctrl+r | reverse lookup of pervious commands |
| !!     | repeat last command |
| exit   | log out of current session |

