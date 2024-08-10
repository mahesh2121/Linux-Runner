
2:37 How to set a username and password to never expires.
3:37 Why /etc/passwd and /ete/shadow file cannot be merged into 1 file.

To list, all the files opened by particular PID.
=========================================================================================================
lsof -p PID

* We are unable to unmount the file system. What are the reason behind it ?.
=========================================================================================================
You are in the same directory

some users are present in the directory and using its content fuser -cu /dev/sda,

some of the files are open in the directory lsof /dev/sda7


What could be the reason it server take more time after reboot?.
=========================================================================================================
filesystem got corrupt and its ext2,ext2 is not having journaling features


we are trying to create the file under any partition but we are getting permission denied alert. What could be the reason? However space issue and no permission issue?
=========================================================================================================
running out of inode

df -i

df -i /ftpusers/

How to check kernel routing table Information?
=========================================================================================================

route -n

netstat -rn

ip route

How to set sticky bit and what is the difference b/w smalls and capital S 
=========================================================================================================
sticky bit is special permission applied on file and directory than only root and owner of that file or directory can deleteit. Even if others having full permission.


Symbolic way:

chmod o+t /opt/dump/

chmod +t /opt/dump/

Numerical way:

chmod 1757 /opt/dump/

To make this setuid executale you have 

chmod 4700 executable

als

s- setuid and executable

S- setuid and non-executable
