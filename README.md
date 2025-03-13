
**Group:** RPZ-23A  
**Student:** Slobozhan Sofiia  

Here is the translation of your text into English:

# Laboratory Work Report

## Title Page
**Topic:** Familiarization with navigation commands in the file system and file and directory management  
**Objective:**  
- To acquire practical skills in working with the Bash command shell.  
- To get acquainted with basic navigation commands in the file system.  
- To learn basic commands for managing files and directories.  

## Preliminary Preparation Tasks

### Glossary of Terms
1. **pwd** - command that shows the current working directory (print working directory).
2. **cd** - command to change the directory (change directory).
3. **ls** - command to view the contents of a directory (list).
4. **cp** - command to copy files (copy).
5. **mv** - command to move or rename files (move).
6. **rm** - command to delete files (remove).
7. **mkdir** - command to create a new directory (make directory).
8. **touch** - command to create an empty file or change the modification time of a file (create or update file).
9. **echo** - command to output text to the terminal or to a file.

### Answers to Questions

#### 2.1. Comparison of File Structures in Windows-like and Linux-like Systems
- **Windows:** The file structure is organized hierarchically, with the top level called "My Computer," and physical devices have letters (C:, D:, etc.). Each disk has its root, and files are organized into folders.
- **Linux:** The file structure starts from the root directory, denoted by the symbol "/", and all devices are accessible through directories, without using letters. The structure is more unified, as all files, including devices, are represented as files in a hierarchy.

#### 2.2. Concept of FHS
FHS (Filesystem Hierarchy Standard) is a standard that defines the directory structure in the Linux file system. It provides a unified organization of files and directories, making navigation and system management easier. Many Linux distributions adhere to this standard, allowing users to easily find files.

#### 2.3. Basic Commands for Working with Files and Directories in Linux
- **Creation:** `mkdir [directory_name]`, `touch [file_name]`
- **Moving:** `mv [source] [destination]`
- **Copying:** `cp [source] [destination]`
- **Deleting:** `rm [file_name]`, `rmdir [directory_name]`, `rm -r [directory_name]`

## Main Positions of the Work Process

| Command Name | Purpose and Functionality |
|--------------|----------------------------|
| `pwd`        | Determines the user's location in the file system, shows the current working directory. |
| `cd Documents` | Changes to the "Documents" directory. |
| `ls -l`      | Views the contents of the current directory in long format. |
| `ls -a`      | Views the contents of the directory, including hidden files. |
| `mkdir [group_name]` | Creates a new directory named after the group. |
| `touch lab5` | Creates an empty file lab5. |
| `echo "Hello, my name is Name1" > name1` | Writes information about the student to the file name1. |
| `cat name1`  | Views the contents of the file name1. |
| `cp name1 name2` | Copies the file name1 to the file name2. |
| `mv name2 surname2/` | Moves the file name2 to the directory surname2. |
| `rm -r [directory_name]` | Deletes the directory along with all its contents. |

---

## **Part 1: Command Table**

| Command Name                            | Purpose and Functionality                                                                                         |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `pwd`                                    | Determines the user's location in the file system, displaying the current working directory (print working directory). |
| `cd Documents`                           | Moves to the "Documents" directory.                                                                              |
| `cd /`                                   | Moves to the root directory.                                                                                     |
| `cd /home`                               | Moves to the users' directory.                                                                                   |
| `cd ~`                                   | Moves to the current user's home directory.                                                                      |
| `cd` (no argument)                       | Same as `cd ~`, returns to the home directory.                                                                  |
| `cd ..`                                  | Moves one level up in the file system.                                                                          |
| `cd ../..`                               | Moves two levels up.                                                                                            |
| `cd -`                                   | Moves to the previous directory.                                                                                |
| `ls -l`                                  | Displays the contents of a directory in long format.                                                            |
| `ls -a`                                  | Displays the contents of a directory, including hidden files.                                                   |
| `ls -R`                                  | Recursively displays the directory contents (including subdirectories).                                         |
| `ls -r`                                  | Displays the contents in reverse alphabetical order.                                                            |
| `ls /etc/[S]`                            | Displays files in the /etc directory that start with the letter "S".                                            |
| `ls /etc/??????`                         | Displays files in the /etc directory whose names consist of six letters.                                        |
| `ls /etc/*[s]`                           | Displays files in the /etc directory whose names end with "s".                                                 |
| `mkdir RPZ-23A`                          | Creates a directory named after the group.                                                                     |
| `touch lab5`                             | Creates an empty file "lab5".                                                                                   |
| `mkdir Slobozhan1 Slobozhan2 Slobozhan3` | Creates three directories with the student's surname.                                                           |
| `echo "Hello, my name is Sofiia" > Sofiia` | Writes text to the file Sofiia.                                                                                |
| `cat Sofiia`                              | Displays the contents of the file Sofiia.                                                                     |
| `cp Sofiia Sofiia2`                        | Copies the file Sofiia to Sofiia2.                                                                             |
| `mv Sofiia2 Slobozhan2/`                  | Moves the file Sofiia2 to the Slobozhan2 directory.                                                            |
| `mv Sofiia3 Slobozhan3/`                  | Moves the file Sofiia3 to the Slobozhan3 directory.                                                            |
| `ls -R RPZ-23A`                          | Displays the directory contents with subdirectories, including color coding.                                   |

---

## **Part 2: Executing Commands in the Terminal**

1. **Determine the current directory:**
   ```bash
   pwd
   ```

2. **Move to the root directory and check the location:**
   ```bash
   cd /
   pwd
   ```

3. **View the contents of the directory in long format:**
   ```bash
   ls -l
   ```

4. **Move to the /usr/share directory and verify the current directory:**
   ```bash
   cd /usr/share
   pwd
   ```

5. **View the contents of the directory, including hidden files:**
   ```bash
   ls -a
   ```

6. **Move to the /etc directory and filter files:**
   ```bash
   cd /etc
   ls S*
   ls ??????
   ls *s
   ```

7. **Move to the home directory and view its contents recursively:**
   ```bash
   cd ~
   ls -R | sort -r
   ```

8. **Create the group directory and verify:**
   ```bash
   mkdir RPZ-23A
   ls -r
   ```

9. **Create files and directories:**
   ```bash
   cd RPZ-23A
   touch lab5
   mkdir Slobozhan1 Slobozhan2 Slobozhan3
   cd Slobozhan1
   touch Sofiia
   echo "Hello, my name is Sofiia" > Sofiia
   cat Sofiia
   ```

10. **Copying, moving, and editing files:**
    ```bash
    cp Sofiia Sofiia2
    mv Sofiia2 ../Slobozhan2/
    cp Sofiia Sofiia3
    mv Sofiia3 ../Slobozhan3/
    cd ../Slobozhan3
    cat Sofiia3
    echo "Hello, my name is Sofiia" > Sofiia3
    cat Sofiia3
    ```

11. **Viewing the structure of created directories:**
    ```bash
    cd ~
    ls -R RPZ-23A
    ```
    Image:
    ![image](https://github.com/user-attachments/assets/90c5ee87-0f0f-4b7e-b4b6-e5a9c0b29e5c)
    ![image](https://github.com/user-attachments/assets/1cbc484f-03c9-4d50-9533-96e4508f898e)



---

**Laboratory work completed by:**  
**Slobozhan Sofiia, Group RPZ-23A**



## Answers to Control Questions

1. **How can you view the path to the user's home directory using the echo command?**
   - `echo $HOME`
   - `echo ~`

2. **Can you view the contents of the root directory while in the user's home directory without going to the root directory?**
   - Yes, you can use the command `ls /`.

3. **How can you add information to an empty file in the terminal?**
   - By using the command `echo "text" > filename`.

4. **How to copy and delete an existing directory? Will there be a difference in commands if the directory is not empty?**
   - To copy: `cp -r [source_directory] [destination_directory]`.
   - To delete: `rm -r [directory_name]` (for a non-empty directory).

5. **In which of the following examples does a file move occur? Its renaming? Both actions simultaneously?**
   - `mv /work/tech/comp.png /Desktop` - moving.
   - `mv /work/tech/comp.png /work/tech/my_car.png` - renaming.
   - `mv /work/tech/comp.png /Desktop/computer.png` - both actions simultaneously.

## Conclusions from the Work Results
During the laboratory work, I became familiar with the basic commands for navigation and file management in Linux. I learned to use the command line to perform various operations such as creating, copying, moving, and deleting files and directories. These skills are important for effective work in the Linux environment, as the command line provides more opportunities and control compared to graphical interfaces.
