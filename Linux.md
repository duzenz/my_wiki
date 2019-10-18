# Disk Usage Commands

```bash
du -sh folder_name
```

```bash
dh -f
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


