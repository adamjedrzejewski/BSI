# Deleted file

1. `ssh <user>@<ip>`
2. `ps -x` get the pid of python program, number of first column
3. `ls -l /proc/<pid>/fd`, list descriptors, one of the descriptors will point to deleted file
4. `cat /proc/<pid>/fd/<descriptor>`