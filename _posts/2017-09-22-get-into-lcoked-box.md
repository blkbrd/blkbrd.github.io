#Unlocking a laptop when you forgot the password 

I recently forgot a password for my hard drive and had to reset it. 
A friend showed me a cool way to change the password for my Windows Hard Drive. 
Simply, the steps are as follows: 
1. Plug drive into another host via SATA/write blocker cable
2. Decrypt drive as needed
3. Run PowerShell as an Admin
  1. take ownership of utilman.exe and cmd.exe in System32
4. change file permissions on those 'exe's as needed
5. rename utilman.exe to utilman1.exe
6. rename cmd.exe to utilman.exe
7. Plug Hard Drive into hardware and boot
8. press 'win' + 'u' and a command prompt will appear
9. net user <user> <pass> to reset password 
10. log in and fix executable names to original!

