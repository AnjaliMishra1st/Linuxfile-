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


























