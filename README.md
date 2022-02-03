# Linux_commands
Useful Linux commands

### File Commands
| Command                 | Result                              |
| :---------------------: | :-----------------------------------|
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

### SSH

| Command                     | Result                              |
| :-------------------------: | :-----------------------------------|
| ssh user@server_ip          | connect to server_ip host as user |
| ssh -p 8888 user@ server_ip | connect to server_ip host as user using port 8888 |
| ssh -D 8889 user@ server_ip | connect to server_ip host as user using bind port 8889 |

### INSTALLATION
| Command      | Result                  |
| :----------: | :-----------------------|
| ./install    | run the install script  |
| make         | ---                     |
| make install | ---                     |

### NETWORK
| Command            | Result                    |
| :----------------: | :------------------------ |
| ping host          | ping host                 |
| whois google.com   | get whois for google.com  |
| dig google.com     | get DNS for google.com    |
| dig -x 192.168.1.1 | reverse lookup host       |
| wget file          | download file             |
| wget -c file       | continue stopped download |
| wget -r url        | recursively download file from URL |

### SYSTEM INFO

| Command            | Result                    |
| :----------------: | :------------------------ |
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
| :---------------------: | :------------------------------------ |
| grep pattern file.txt   | search for pattern in file.txt        |
| grep -r pattern dir     | search recursively for pattern in dir |
| command \| grep pattern | search the pattern in the output of the command |
