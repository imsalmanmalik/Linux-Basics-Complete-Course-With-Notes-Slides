# Lab - Working with shell

1. To check the home directory for a particular user say **`salman`**
   ```
   $ grep salman /etc/passwd | cut -d ":" -f6
   ```
1. To check the home directory for a particular user using built in shell variables
   ```
   $ echo $HOME
   ```
1. In the command **`echo Welcome`**, what does the word Welcome represent with respect to the command?
   ```
   $ echo Welcome 
     - Where Welcome is an argument
   ```
   
1. To check **`git`** command type
   ```
   $ type git
   ```
1. To create a directory
   ```
   $ mkdir /home/salman/birds
   ```
1. To create directories recursively
   ```
   $  mkdir -p /home/salman/fish/salmon
   ```
1. Create few more directories
   ```
   $ mkdir -p /home/salman/mammals/elephant
   $ mkdir -p /home/salman/mammals/monkey
   $ mkdir /home/salman/birds/eagle
   $ mkdir -p /home/salman/reptile/snake
   $ mkdir -p /home/salman/reptile/frog
   $ mkdir -p /home/salman/amphibian/salamander
   ```
1. To move a directory
   ```
   $ mv /home/salman/reptile/frog /home/salman/amphibian
   ```
1. To rename a directory
   ```
   $ mv /home/salman/reptile/snake /home/salman/reptile/crocodile
   ```
1. To delete a directory
   ```
   $ rm -r /home/salman/reptile
   ```
