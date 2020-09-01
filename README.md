# borg-btrfs-backup
borg-btrfs-backup is a script, backing up the files of a btrfs filesystem by creating a snapshot. After every backup, the script sends an email with the status of the backup and the log file. It also creates a timestamp file to monitor the last successful backup by the timestamp of that file. The script needs to be run as root.

The only argument given to borg-lvm-backup.sh is the name of the config file of the specific job located in ./config/ folder. The name of the config file is also the jobname, located in the archive name.

For mail sending the programm sendemail and the libarys perl libaries Net::SSLeay and IO::Socket::SSL need to be installed. Under debian and ubuntu, this can be done with "apt install sendemail libnet-ssleay-perl libio-socket-ssl-perl".
