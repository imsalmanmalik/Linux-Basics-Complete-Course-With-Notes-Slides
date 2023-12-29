# Lab - Linux Bash Shell

1. To check the default shell for the current user. Display the shell for the current user but not necessarily the shell that is running at the movement.
   ```
   $ echo $SHELL
   ```
2. To change the shell for salman from **`Bash`** to **`Bourne Shell`**
   ```
   $ chsh -s /bin/sh salman
   ```
3. What is the value of the environment variable **`TERM`**
   ```
   echo $TERM
   ```  
4. Create a new environment variable called **`PROJECT=MERCURY`** and make it persistent by adding the variable to the **`~/.profile`** file.
   ```
   echo export PROJECT=MERCURY >> ~/.profile
   ```
5. Which of the following directories is not part of the PATH variable?
   ```
   /opt/salman-code
   ```
6. Set an alias called **`up`** for the command **`uptime`** and make it persistent by adding to **`~/.profile`** file.
   ```
   echo alias up=uptime >> ~/.profile
   ```
