su betty: switch user to betty
whoami : prints the effective username of the current user
groups : prints all the groups the user is part in
chown hello betty : set first the file to be owner-changed, then the new owner.
touch hello : creates a new empty file called "hello"
chmod 700 hello : give the acces to execute the file to the owner itself.
chmod 754 hello : grant all the permissions to the owner, read and execute to the group and only read to the other users.
chmod 555 hello :
ch mod 007 hello :
chmod 753 hello :
chmod --reference=olleh hello : take reference from the "olleh" file.
chmod -R a+x /holbertonschool-shell/permissions : adds execute permisions to all in the subdirectories of the designed directory.
mkdir -m u=rwx,g=rx,o=x my_dir : creates a directory whit the assigned permissions.
chgrp school hello : change the group to school for the file "hello"
chown -R vincent[:staff] /holbertonschool-shell/permissions :
