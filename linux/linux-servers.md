# Intro to Linux for Servers

Linux is an operating system, like OS X or Microsoft. By some estimates Linux accounts for 80% of server operating systems.

Linux has 100 of distributions.

Free as in beer refers to money. Just because you get to use it for free, doesn’t mean that you get to see the underlying source code or modify it for your own purposes. 

Free as in speech refers to your rights. You are free to run the software, see how it runs, modify it, improve upon, and distribute it.

Linux became popular because it was free as in speech.

###Choosing the right distro:

**Redhat** Enterprise: Need to pay a licensing fee - and receive support

**ubuntu**: various distros (desktop, serve, mobile); it receives consistent updates to its software

**debian**: is known for stability and reliability; software update cycle is very slow when compared to others

**CoreOS**: clusters of containerized apps

###Vagrant Commands

`vagrant up`: start virtual machine
`vagrant status`: show the status of the virtual machine 
`vagrant suspend`: saves all work and puts machine into sleep mode
`vagrant ssh`: connect to and log into the virtual machine
`vagrant halt`: halts/turns off machine; frees up all RAM
`vagrant destroy`: destroys virtual machine; work is not saved; formatting hard drive

###Where we are in the terminal

Use `ls -al` to see all files -- including the hidden ones.

If the first character is a `d` it is a directory. If the first character is a `-` it is a file.

###Important Directories
To get to the top level root folder `cd /`.

`etc`: is where configuration files live

`var`: is where variable files live; variable files are files which you expect to grow or change in size over time; typically system and application logs within here

`bin`: is where executable binaries are stored; these are accessible by all users; apps you run like `ls`

`sbin`: similar to `bin` but only to be used by the root user for system admin and maintenance  

`lib`: libraries that support the binaries around a system

`usr`: user programs; binaries aren't required for bootup or system maintenance

###Understanding $PATH

Linux provides a shortcut system within the $PATH variable. 

Running `echo $PATH` presents you with a bunch of paths separated by `:` characters.

```bash
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games
```

These are the directories that Linux will look through when you type a command like `ls`. The operating system checks the directories until it finds the executable file.