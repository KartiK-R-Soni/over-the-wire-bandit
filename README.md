# over-the-wire-bandit
Level 1-Code# ls->cat readme
Ls is the command to list files.
Cat is used to read input from the file and give output

ssh bandit1@localhost->to shift to bandit2

Level 1-Code ls->cat ./-
As the filename starts from a - it would add a flag but we want to read the file - so we would add .

ssh bandit2@localhost->to shift to bandit3


Level 2-Code  ls->cat "spaces in this filename"
Simply writing spaces in the filename would take spaces,in,this,filename as diffrent arguement and will give error

ssh bandit3@localhost->to shift to bandit4

Level 3-Code ls -> cd inhere -> ls -apl -> cat .hidden

ssh bandit4@localhost->to shift to bandit5

Level 4-Code ls -> cd inhere -> ls -apl -> find ./-* -> cat 

ssh bandit5@localhost->to shift to bandit6

Level 5-Code ls -> cd inhere -> ls apl -> find -size 1033c -> cat ./maybehere07/.file2 


ssh bandit6@localhost->to shift to bandit7

Level 6-Code pwd -> find / -user bandit 7 -group bandit 6  size -33c
->/var/lib/dpkg/info/bandit7.password

ssh bandit7@localhost->to shift to bandit8

Level 7-Code ls -> cat data.txt | grep="millionth"

ssh bandit8@localhost->to shift to bandit8

Level 8-Code ls -> cat data.txt | sort | uniq -u

ssh bandit9@localhost->to shift to bandit9

 Level 9-Code ls -> file data.txt -> cat data.txt -> strings data.txt | grep "=="

ssh bandit10@localhost->to shift to bandit8

Level 10-Code ls -> cat data.txt -> base64 -d data.txt

