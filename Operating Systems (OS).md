# Operating Systems (OS)

![c](https://user-images.githubusercontent.com/116082827/235295355-e2b55f7a-b3a8-499e-b0a1-3fab9022d941.png)


An operating system is the software that manages computer hardware and software resources and provides common services for computer programs. Understanding how an OS works is essential for developing software that interacts with the underlying system. Here's an example of a simple OS operation in Python using the os library:



import os



# Get the current working directory

cwd = os.getcwd()

print('Current working directory:', cwd)



# Create a new directory

os.mkdir('new_dir')



# Change the current working directory

os.chdir('new_dir')

print('New current working directory:', os.getcwd())



# Delete the directory

os.chdir('..')

os.rmdir('new_dir')
