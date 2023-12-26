- 👋 Hi, I’m @Hacker77DL
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Hacker77DL/Hacker77DL is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#!/bin/bash

if["$1"==""]
then
echo "you forget an ip address!"
echo syntax:  ./ipsweep.sh  192.168.1"
 else
 for ip in 'seq 1 254';  do
 ping -c 1 $1.$ip| grep "64 bytes" | cut-d" " -f 4| tr-d ":"&
 done 
 fi
