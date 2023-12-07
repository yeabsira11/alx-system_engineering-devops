0x01. Shell, permissions

0.	Create a script that switches the current user to the user betty.
	#!/bin/bash
	su betty
1.	Write a script that prints the effective username of the current user.
	#!/bin/bash
	whoami
2.	Write a script that prints all the groups the current user is part of.
#!/bin/bash
groups
3.	Write a script that changes the owner of the file hello to the user betty.
#!/bin/bash
chown betty hello
4.	Write a script that creates an empty file called hello.
#!/bin/bash
touch hello
5.	Write a script that adds execute permission to the owner of the file hello.
#!/bin/bash
chmod u+x hello
6.	Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
#!/bin/bash
chmod u+x,g+x,o+r hello
7.	Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello.
#!/bin/bash
chmod a+x hello
8.	Write a script that sets the permission to the file hello as follows:
#!/bin/bash
chmod 007 hello
9.	Write a script that sets the mode of the file hello to this:
#!/bin/bash
chmod 753 hello
10.	Write a script that sets the mode of the file hello the same as olleh’s mode.
#!/bin/bash
chmod --reference=olleh hello
11.	Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.
#!/bin/bash
chmod -R a+x */
12.	Create a script that creates a directory called my_dir with permissions 751 in the working directory.
#!/bin/bash
mkdir -m 751 my_dir 
13.	Write a script that changes the group owner to school for the file hello.
#!/bin/bash
chgrp my_dir hello
14.	Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
#!/bin/bash
chown betty:my_dir *
15.	Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.
#!/bin/bash
chown -h betty:My_dir _hello
16.	Write a script that changes the owner of the file hello to betty only if it is owned by the user guillaume.
#!/bin/bash
chown --from=guillaume betty hello
17.	Write a script that will play the StarWars IV episode in the terminal.
#!/bin/bash
telnet towel.blinkenlights.nl




