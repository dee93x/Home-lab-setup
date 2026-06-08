# Home Lab Setup

## Overview
A personal home lab built using VirtualBox and Ubuntu Linux to practise IT support skills.

## Environment
- Host OS: Windows 11
- Virtualisation: Oracle VirtualBox
- Guest OS: Ubuntu 24.04 LTS

## Tasks Completed
- [x] Task 1 — Terminal navigation and file management
- [x] Task 2 — Network diagnostics
- [x] Task 3 — User and permission management
- [x] Task 4 — Installing software with APT
- [ ] Task 5 — System log analysis
- [ ] Task 6 — Process monitoring

## What I Learned
       
       LEARNING TERMINAL BASIC COMMANDS
       pwd              ← shows where you are (current folder)
       ls               ← lists files in current folder
       ls -la           ← lists ALL files with details
       cd Documents     ← move into Documents folder
       cd ..            ← go back up one level
       mkdir myfolder   ← create a new folder called "myfolder"
       cd myfolder      ← go into it
       touch test.txt   ← create an empty file called test.txt
       ls               ← you should see test.txt listed
       cat test.txt     ← display file contents (empty for now)
       echo "Hello" > test.txt   ← write "Hello" into the file
       cat test.txt     ← now you should see "Hello"
       rm test.txt      ← delete the file
       ls               ← confirm it's gone

       CHECKING NETWORK PERMISSIONS
       ip a              ← shows your IP address and network interfaces
       ping google.com   ← tests internet connection (press Ctrl+C to stop)
       nslookup google.com  ← looks up Google's IP address via DNS
       traceroute google.com  ← shows the path data takes to Google
       sudo apt install traceroute   ← installs it (enter your password when asked)
      
       MANAGING USERS & PERMISSIONS
       whoami                        ← shows your current username
       sudo adduser testuser         ← creates a new user called "testuser"
                                    (follow the prompts, set a password)
       cat /etc/passwd               ← shows all users on the system
       ls -la /home                  ← shows home folders for each user
       sudo userdel testuser         ← delete the test user when done
       
       CREATING FILE AND CHANGING PERMISSIONS
       touch myfile.txt
       ls -la myfile.txt             ← note the permissions (e.g. -rw-r--r--)
       chmod 777 myfile.txt          ← give everyone full access
       ls -la myfile.txt             ← see how permissions changed
       chmod 644 myfile.txt          ← set back to normal
       ls -la myfile.txt             ← confirm change

       INSTALLING AND REMOVING SOFTWARE 
       sudo apt update              ← refresh the list of available software
       sudo apt install htop        ← install a system monitor tool
       htop                         ← open it (press Q to quit)
       sudo apt install net-tools   ← install classic network tools
       ifconfig                     ← now this command works (like ip a)
       sudo apt remove htop         ← uninstall htop
       

       



       
     
       
