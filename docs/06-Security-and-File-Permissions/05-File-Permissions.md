# LINUX FILE PERMISSIONS

  - In this lecture we will learn about various file type identifiers.
  - We will also learn about various Linux file permissions that can be applied on the file or the directory.

    ![perm](../../images//perm.PNG)


    ![type](../../images//type.PNG)


  #### Directory Permission

  - To list the directory permission use

    ```
    [~]$ ls -ld /home/salman/random_dir
    ```

  - To know the current user 

    ```
    [~]$ whoami
    ```
 
  - To change the change the directory

    ```
    [~]$ cd /home/salman/random_dir
    ```

  #### File Permissions

  - Linux file permissions are defined as 

    ![filep](../../images//filep.PNG)

  #### Modifying file permissions

  - Use **`chmod`** command to modify the file permissions.

  - Provide full access to owners

    ```
    [~]$ chmod u+rwx test-file
    ```

  - Provide Read access to Owners, groups and others, Remove execute access

    ```
    [~]$ chmod ugo+r-x test-file
    ```

  - Remove all access for others

     ```
     [~]$ chmod o-rwx test-file
     ```

  - Full access for Owner, add read , remove execute for group and no access for others

    ```
    [~]$ chmod u+rwx,g+r-x,o-rwx test-file
    ```
 
  - Provide full access to Owners, group and others

    ```
    [~]$ chmod 777 test-file
    ```

  - Provide Read and execute access to Owners,groups and others

    ```
    [~]$ chmod 777 test-file
    ```

  - Read and Write access for Owner and Group, No access for others.

    ```
    [~]$ chmod 660 test-file
    ```

  - Full access for Owner, read and execute for group and no access for others.

    ```
    [~]$ chmod 750 test-file
    ```

  #### Change Ownership 
   
  - Changes owner to salman and group to developer
   
    ```
    [~]$ chown salman:developer test-file
    ```
    
  - Changes just the owner of the file to salman. Group unchanged.

    ```
    [~]$ chown salman andoid.apk
    ```

  - Change the group for the test-file to the group called android. 

    ```
    [~]$ chgrp android test-file
    ```
