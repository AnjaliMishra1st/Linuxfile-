# Linuxfile-
linux for devops
anjali@ubuntu:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
anjali@ubuntu:~$ mkdir devops
anjali@ubuntu:~$ ls
Desktop  Documents  Music     Public     Videos
devops   Downloads  Pictures  Templates
anjali@ubuntu:~$ ls -l
total 36
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Desktop
drwxrwxr-x 2 anjali anjali 4096 Jun  5 03:25 devops
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Documents
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Downloads
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Music
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Pictures
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Public
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Templates
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Videos
anjali@ubuntu:~$ pwd
/home/anjali
anjali@ubuntu:~$ touch newfile.txt
anjali@ubuntu:~$ ls
Desktop  Documents  Music        Pictures  Templates
devops   Downloads  newfile.txt  Public    Videos
anjali@ubuntu:~$ cd
anjali@ubuntu:~$ touch devops_file.txt
anjali@ubuntu:~$ rm devops_file.txt
anjali@ubuntu:~$ ls
Desktop  Documents  Music        Pictures  Templates
devops   Downloads  newfile.txt  Public    Videos
anjali@ubuntu:~$ touch demofile.txt 
anjali@ubuntu:~$ ls
demofile.txt  devops     Downloads  newfile.txt  Public     Videos
Desktop       Documents  Music      Pictures     Templates
anjali@ubuntu:~$ cat demofile.txt
anjali@ubuntu:~$ echo "hello dosto"
hello dosto
anjali@ubuntu:~$ echo "hello dosto"> demofile.txt
anjali@ubuntu:~$ cat demofile.txt
hello dosto
anjali@ubuntu:~$ echo "this is my file" > myfile.txt
anjali@ubuntu:~$ ls
demofile.txt  devops     Downloads  myfile.txt   Pictures  Templates
Desktop       Documents  Music      newfile.txt  Public    Videos
anjali@ubuntu:~$ cat newfile.txt
anjali@ubuntu:~$ cat myfile.txt
this is my file
anjali@ubuntu:~$ head myfile.txt
this is my file
anjali@ubuntu:~$ tail myfile.txt
this is my file
anjali@ubuntu:~$ tail -f myfile.txt
this is my file


anjali@ubuntu:~$ ls
demofile.txt  devops.txt  Music        Pictures   Videos
Desktop       Documents   myfile.txt   Public
devops        Downloads   newfile.txt  Templates
anjali@ubuntu:~$ myfile.txt
myfile.txt: command not found
anjali@ubuntu:~$ touch myfile.txt
anjali@ubuntu:~$ cat myfile.txt
this is my file
anjali@ubuntu:~$ wc myfile.txt
 1  4 16 myfile.txt
anjali@ubuntu:~$ ls -l
total 44
-rw-rw-r-- 1 anjali anjali   12 Jun  5 03:52 demofile.txt
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Desktop
drwxrwxr-x 3 anjali anjali 4096 Jun  5 04:44 devops
-rw-rw-r-- 1 anjali anjali    0 Jun  5 04:32 devops.txt
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Documents
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Downloads
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Music
-rw-rw-r-- 1 anjali anjali   16 Jun 16 06:15 myfile.txt
-rw-rw-r-- 1 anjali anjali    0 Jun  5 03:26 newfile.txt
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Pictures
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Public
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Templates
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Videos
anjali@ubuntu:~$ ls
demofile.txt  devops.txt  Music        Pictures   Videos
Desktop       Documents   myfile.txt   Public
devops        Downloads   newfile.txt  Templates
anjali@ubuntu:~$ cd linux_for_devops/
bash: cd: linux_for_devops/: No such file or directory
anjali@ubuntu:~$ myfile.txt cd cloud
myfile.txt: command not found
anjali@ubuntu:~$ myfile.txt newfile.txt
myfile.txt: command not found
anjali@ubuntu:~$ echo "hello dosto, this is soft link"
hello dosto, this is soft link
anjali@ubuntu:~$ touch devops-file.txt
anjali@ubuntu:~$ ^C
anjali@ubuntu:~$ devops-file pwd
devops-file: command not found
anjali@ubuntu:~$ ln hardlink-file ^C
anjali@ubuntu:~$ ln hardlink-file devops-file
ln: failed to access 'hardlink-file': No such file or directory
anjali@ubuntu:~$ ^C
anjali@ubuntu:~$ ln hardlink-file devops
ln: failed to access 'hardlink-file': No such file or directory
anjali@ubuntu:~$ 
anjali@ubuntu:~$ touch linux_for_devops
anjali@ubuntu:~$ ls
demofile.txt  devops-file.txt  Downloads         myfile.txt   Public
Desktop       devops.txt       linux_for_devops  newfile.txt  Templates
devops        Documents        Music             Pictures     Videos
anjali@ubuntu:~$ ln -s /home/ubuntu/linux_for_devops/cloud/devops-file.txt
ln: failed to create symbolic link './devops-file.txt': File exists
anjali@ubuntu:~$ ln -s /home/ubuntu/linux_for_devops/devops-file.txt softlink-file
anjali@ubuntu:~$ ls
demofile.txt     devops.txt        Music        Public
Desktop          Documents         myfile.txt   softlink-file
devops           Downloads         newfile.txt  Templates
devops-file.txt  linux_for_devops  Pictures     Videos
anjali@ubuntu:~$ ls -ltr
total 44
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Videos
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Templates
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Public
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Pictures
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Music
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Downloads
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Documents
drwxr-xr-x 2 anjali anjali 4096 Jun  5 03:23 Desktop
-rw-rw-r-- 1 anjali anjali    0 Jun  5 03:26 newfile.txt
-rw-rw-r-- 1 anjali anjali   12 Jun  5 03:52 demofile.txt
-rw-rw-r-- 1 anjali anjali    0 Jun  5 04:32 devops.txt
drwxrwxr-x 3 anjali anjali 4096 Jun  5 04:44 devops
-rw-rw-r-- 1 anjali anjali   16 Jun 16 06:15 myfile.txt
-rw-rw-r-- 1 anjali anjali    0 Jun 16 06:31 devops-file.txt
-rw-rw-r-- 1 anjali anjali    0 Jun 16 06:44 linux_for_devops
lrwxrwxrwx 1 anjali anjali   45 Jun 16 06:49 softlink-file -> /home/ubuntu/linux_for_devops/devops-file.txt
anjali@ubuntu:~$ cat softlink-file
cat: softlink-file: No such file or directory
anjali@ubuntu:~$ cd devops
anjali@ubuntu:~/devops$ cd linux_for_devops
bash: cd: linux_for_devops: No such file or directory
anjali@ubuntu:~/devops$ echo "this file was changed">
bash: syntax error near unexpected token `newline'
anjali@ubuntu:~/devops$ echo "this file was changed"
this file was changed
anjali@ubuntu:~/devops$ 




























