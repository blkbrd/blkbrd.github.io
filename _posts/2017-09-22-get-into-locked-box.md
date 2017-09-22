---
layout: post
title: "Get into a Windows laptop without the password"
date: 2017-09-22
---

I recently forgot a password for my Windows Hard Drive and had to reset it. 
A friend showed me a cool way to change the password for my hard drive. 
Simply, the steps are as follows: 
1. Plug drive into another host via SATA/write blocker cable
2. Decrypt drive as needed
3. Run PowerShell as an Admin
  1. take ownership of utilman.exe and cmd.exe in System32
  2. change file permissions on those 'exe's as needed
  3. rename utilman.exe to utilman1.exe
  4. rename cmd.exe to utilman.exe
4. Plug Hard Drive into hardware and boot
5. Press 'win' + 'u' and a command prompt will appear
6. <code> net user USER PASS </code> to reset password 
7. log in and fix executable names to original!

