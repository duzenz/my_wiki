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

