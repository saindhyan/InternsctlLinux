# xenonModule-3

# Scenario
## There is a customer who came to you with a problem to have a custom linux command for his operations. Your task is to understand the problem and create a linux command via bash script as per the instructions.
Command name - internsctl
Command version - v0.1.0

## Script flow
![flow](https://github.com/saindhyan/internsctl/assets/87525527/2f956d97-f5fd-4645-9b6d-3dcd52a428dd)

## step 1 Place script file to /bin folder
```
$ sudo mv internsctl /bin/internsctl
```
## step 2 Provide executable permission to file
```
$ sudo chmod +x internsctl
```
## step 2 Place manual file to /usr/share/man/man1 folder
```
$ sudo mv internsctl /usr/share/man/man1/internsctl
```

## Command :
``` 
$ man internsctl
```
It will provide the user manual for the cammand/script 
It will provide all the details about this script


## Command :
```
$ internsctl --help
 ```

-  --help     Display help and examples
  



## Command :
```
$ internsctl --version
```
- --version  Display command version

## Command 
```
$ internsctl memory getinfo
```
-  memory getinfo         : Get memory information of the server.


## Command :
```
$ internsctl cpu getinfo
```

-  cpu getinfo  : Get CPU information of the server.

## Command :
```
$ internsctl user create piyush
```

-  user create piyush : Create a new user with the given username i.e. piyush.
## Command :
```
$ internsctl user list
```

-  user list : List all regular users present on the server.




## Command
```
$ internsctl user list --sudo-only
```

-  user list --sudo-only  : List all users with sudo permissions on the server.
 result : piyush

## Command :
```
$ internsctl file getinfo file.txt
```

-  file getinfo file.txt : Get File.txt Info

## Command $ internsctl file getinfo [options] file.txt

-  --size, -s to print size
    example :
  ```
   $internsctl file grtinfo --size file.txt
   ```


-  --permissions, -p print file permissions
    example :
   ```
    $internsctl file grtinfo --permissions file.txt
   ```


-  --owner, o print file owner
  example :
```
 $internsctl file grtinfo --owner file.txt
```

-  --last-modified, m
    example :
   ```
   $internsctl file grtinfo --last-modified file.txt
   ```


