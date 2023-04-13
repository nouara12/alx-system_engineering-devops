Prints the absolute path name of the current working directory
#!/bin/bash
pwd

Display the contents list of your current directory
#!/bin/bash
ls

Changes the working directory to the user’s home directory
#!/bin/bash
cd ~

Display current directory contents in a long format
#!/bin/bash
ls -l

Display current directory contents, including hidden files
#!/bin/bash
ls -al

Display current directory contents
#!/bin/bash
ls -lan

Create a script that creates a directory named my_first_directory in the /tmp/ directory
#!/bin/bash
mkdir /tmp/my_first_directory

Move the file betty from /tmp/ to /tmp/my_first_directory
#!/bin/bash
mv /tmp/betty /tmp/my_first_directory

Delete the file betty
#!/bin/bash
rm /tmp/my_first_directory/betty

Delete the directory my_first_directory that is in the /tmp directory
#!/bin/bash
rm -r /tmp/my_first_directory

Write a script that changes the working directory to the previous one
#!/bin/bash
cd –

Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format
#!/bin/bash
ls -la . .. /boot

Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script
#!/bin/bash
file /tmp/iamafile

Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory
#!/bin/bash
ln -s /bin/ls __ls__

Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory
#!/bin/bash
cp -un *.html ../

