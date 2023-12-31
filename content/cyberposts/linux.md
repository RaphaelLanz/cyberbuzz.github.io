---
title: "Linux"
date: 2023-07-07T19:28:01+01:00
draft: true
---

# What is Linux?
Linux is an open-source operating system that was created by Linus Torvalds in 1991. It is a free and highly customizable alternative to commercial operating systems like Windows and macOS. Linux is known for its stability, security, and flexibility, and it is widely used on various devices, ranging from servers and supercomputers to desktop computers, laptops, and even smartphones.

What sets Linux apart is its open nature, as its source code is freely available to the public. This allows a large and active community of developers to contribute to its development and improvement. Different distributions, or distros, of Linux exist, each with its own set of features and software packages, but they all share the Linux kernel as their core.

Linux provides both a command-line interface and graphical user interfaces, making it accessible to users of different skill levels. It has a vast ecosystem of free and open-source software applications and strong support for networking and server technologies, making it a popular choice for various purposes, including web hosting, cloud computing, and enterprise solutions. Linux has gained popularity due to its stability, security, and the freedom it provides to its users.

### Basics Linux Commands

Linux commands are instructions given to the Linux operating system to perform various tasks or operations. They are typed into a command line interface, also known as a terminal or console, and executed by the system.

Linux commands can be used to manage files and directories, install and update software packages, configure system settings, network management, process management, user management, and much more.

Most Linux commands have specific syntax, options, and arguments that need to be used correctly in order to achieve the desired results. It’s important to understand the basics of Linux commands if you want to use the Linux operating system effectively.

### pwd:
```bash
pwd: print the name of the current directory

┌──(kali㉿kali)-[~]
└─$ pwd              
/home/kali
```
### cd:
```bash
cd: changed directory

┌──(kali㉿kali)-[~]
└─$ cd Music              

┌──(kali㉿kali)-[~/Music]
└─$ pwd
/home/kali/Music 
```
### whoami:
```bash
 whoami: print the current user

┌──(kali㉿kali)-[~]
└─$ whoami              
kali
```
### clear:
```bash
 clear: clears the terminal

┌──(kali㉿kali)-[~]
└─$               
```

### help:
```
help: show the manual of the command

┌──(kali㉿kali)-[~]
└─$ cat --h or cat --help              

  -A, --show-all           equivalent to -vET
  -b, --number-nonblank    number nonempty output lines, overrides -n
  -e                       equivalent to -vE
  -E, --show-ends          display $ at end of each line
  -n, --number             number all output lines
  -s, --squeeze-blank      suppress repeated empty output lines
  -t                       equivalent to -vT
  -T, --show-tabs          display TAB characters as ^I
  -u                       (ignored)
  -v, --show-nonprinting   use ^ and M- notation, except for LFD and TAB
      --help        display this help and exit
      --version     output version information and exit

Examples:
  cat f - g  Output f's contents, then standard input, then g's contents.
  cat        Copy standard input to standard output.
```

### ls:
```bash
ls: list files and directories in the current directory

┌──(kali㉿kali)-[~]
└─$ ls
 Desktop  Documents  Downloads  Music  overthewire  Pictures  Public  Templates  Videos
```
### cd:
```bash
cd: change directory

┌──(kali㉿kali)-[~]
└─$ cd Documents 
                                                                                                                                                             
┌──(kali㉿kali)-[~/Documents]
└─$ pwd
/home/kali/Documents
```
### touch: 
```bash
touch: create a file without any content

┌──(kali㉿kali)-[~/Documents]
└─$ touch example1 example2

┌──(kali㉿kali)-[~/Documents]
└─$ ls
Desktop  Documents  Downloads  *example1* *example2*  man  Music  overthewire  Pictures  Public  Templates  Videos
```
### mkdir:
```bash
mkdir: make a new directory

┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  Music  overthewire  Pictures  Public  Templates  Videos

┌──(kali㉿kali)-[~]
└─$ mkdir example

┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  *example*  Music  overthewire  Pictures  Public  Templates  Videos
```
### rm:
```bash
rm: delete files or directories
rm -r: recursively delete a directory and all its contents
rm -f: forcibly delete files without asking

┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  *example*  Music  overthewire  Pictures  Public  Templates  Videos

┌──(kali㉿kali)-[~]
└─$ rmdir example

┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  Music  overthewire  Pictures  Public  Templates  Videos
```
### cp:
```bash
cp: copy files and directories

┌──(kali㉿kali)-[~]
└─$ cp example1 example2
```

### mv:
```bash
mv:  moves files and directories from one directory to another or renames a file or directory.
```
### cat:
```bash
cat: maily used to preview a file without opening the text editor
```
### chmod:
```bash
chmod: change the permissions of a file or a directory

chmod 644 file

Read (r) Write (w) Execute (x)

0=No permission
1=Execute
2=Write
4=Read
5=Read and Execute
6=Read and Write
7=Read, Write and Execute
```