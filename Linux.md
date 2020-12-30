# Disk Usage Commands

```bash
du -sh folder_name
```

```bash
dh -f
```

```bash
#show folder sized and sort
du -chd 1 | sort -h
```

# Tar File
```bash
tar czf output_name.tar.gz zipped_folder_name/
```

# Untar File
```bash
tar -xvzf output_name.tar.gz
```

# See Ram Information
```bash
sudo dmidecode --type 17
```


# Network
```bash
ip a | egrep "inet "
```


# Copy file from remote server
```bash
scp remote_username@remote_host:/remote/file.txt /local/directory
scp -i certificate.pem remote_username@remote_host:/remote/file.txt /local/directory
```

# Change root password
```bash
sudo -i
passwd
```

# Change owner
```bash
chown user:group /path/to/file
```

# Kill process on port
```bash
sudo fuser -k {{port}}/tcp
or
sudo kill -9 $(sudo lsof -t -i:9001)
```


# Using snap
```bash
snap find <search_text>
snap install <package>
snap list
snap changes
snap refresh <package>
snap refresh --list
snap remove <package>
```

# Using alias
```bash
alias
alias hede="docker ps"
unalias alias_name

#add your aliases permamnently
vim ~/.bashrc
source ~/.bashrc
```


# list
```bash
-v     natural sort of (version) numbers within text
ls -1v log*

find -type f | wc -l #count of files in a folder
```

# Remove files before a date
```bash
find . -name "*.gz" -type f -mtime +45 -exec rm -f {} \;
```

# grep
```bash
grep "some string" file
grep -i "REact" file #insensitive
grep -c "react" index.js #count
-r recursive
-o only print the matching part the line
-a search binaries
-F dont treat the match string as a regex
-l only show filenames
-v find lines that dont match
-A shows context grep -A 3 foo shows extra 3 lines.
```

#useful commands
```bash
# finding out your 10 most used commands 
history | sed -e 's/ *[0-9][0-9]* *//' | sort | uniq -c | sort -rn | head -10
```


