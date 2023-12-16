## Backup the Server

The script will backup the important directories and save them to `/tmp/backup`


#### Create backup
```sh
bash backup.sh
```


#### Restore backup
To see the list of archived contents:
```sh
tar -tzvf /mnt/backup/host-Monday.tgz
```

To restore a file from the archive to a different directory, enter:

```sh
tar -xzvf /mnt/backup/host-Monday.tgz -C /tmp etc/hosts
```

To restore all files in the archive enter the following:

```sh
cd /
sudo tar -xzvf /mnt/backup/host-Monday.tgz
```
