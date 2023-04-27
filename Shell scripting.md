# Shell scripting 

![l](https://user-images.githubusercontent.com/116082827/234855732-fbc7c4eb-d216-446e-8d46-02be4f7d8fe0.jpeg)


Shell scripting is the process of writing code using a Unix/Linux shell, such as Bash, to automate tasks or perform system administration functions. Shell scripts are text files containing a series of commands that the shell interprets and executes in sequence. They are a powerful tool for automating repetitive tasks, managing files and directories, and running system commands.



Here is an example of a basic shell script in Bash that displays a greeting message:





#!/bin/bash

echo "Hello, world!"

Let's break down this script:



The first line, #!/bin/bash, is called a shebang line, and it specifies which shell the script should be run with (in this case, Bash).

The second line, echo "Hello, world!", is a command that outputs the string "Hello, world!" to the console.

To run this script, save it as a file (e.g. hello.sh) and make it executable with the chmod +x hello.sh command. Then, you can run it with ./hello.sh command.



Here is a more complex example of a shell script that performs a system backup:



bash

Copy code

#!/bin/bash



# Set the backup directory

BACKUP_DIR=/backup



# Create the backup directory if it doesn't exist

if [ ! -d $BACKUP_DIR ]; then

  mkdir $BACKUP_DIR

fi



# Get the current date and time

DATE=`date +%Y-%m-%d_%H-%M-%S`



# Compress the contents of the home directory and store it in the backup directory

tar -czvf $BACKUP_DIR/home_$DATE.tar.gz /home/user



# Remove backups older than 7 days

find $BACKUP_DIR -type f -mtime +7 -exec rm {} \;

Let's break down this script:



The first line is the shebang line, as before.

The second line sets the BACKUP_DIR variable to /backup.

The if statement checks if the backup directory exists, and creates it if it doesn't.

The DATE variable uses the date command to get the current date and time in a specific format.

The tar command compresses the contents of the /home/user directory and saves it in the backup directory with a filename that includes the current date and time.

The find command searches for backup files older than 7 days in the backup directory and removes them.

To run this script, save it as a file (e.g. backup.sh) and make it executable with the chmod +x backup.sh command. Then, you can run it with ./backup.sh command.



Shell scripting can be a powerful tool for automating tasks and managing system resources. There are many resources available online to help you learn more about shell scripting and how to write more complex scripts.
