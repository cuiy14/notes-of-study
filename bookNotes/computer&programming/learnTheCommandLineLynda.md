# Learn the basics of the command line

## chapter 0 Introductions
The basics of the courses. It contains two video showing how to ==install the virtual machine and add the guest additions of the VM==. It can be useful when needed.install the virtual machine and add the guest additions of the VM. It can be useful when needed.

## chapter 1 Command line basics
Some basic thing. Too general.
- some shortcuts
 - to move the cursers -- `^a` `^e` `Ctrl - Left arrow` `Ctrl - Right arrow` `Ctrl U` `Ctrl K` `Ctrl-Shift-C` `Ctrl-Shift-V`
- The command help
 As you ==don't need to memorize everything==, so the method to enquiry commands should be very valuable.
 - `man + command`
 - `command --help`
 - `help` 

## chapter 2 Files, folders and permissions
- `cd -` switch to the previous folder
- `ls -lh` detailed descriptions in the form of lists for human
- `rm -r` means recursive removing things
- `find path -name "fileName"` to find a file with specific name in a specific folder
- `chmod number file` root-group-others
- `chown user file` change the owner of the file

## chapter 3 Common command-line tasks and tools
- `wc` -- to analysis the number of lines,etc,  in a text
- `cat -n file` `echo` `head -n number file` `tail` `more` `less` -- some commands about printing files
- `|` is the pipe; the order matters, ==the output of the left is given to the input of the right==
- `grep -n "String" file` -- parse the text, support the regular expression, other options like -i or -v or -E, etc.
-  `awk` `sed` `tr` `sort` -- to manipulate the text stream
- `tar` -- to archive and extract some files
- stdin(0) \ stdout(1) \ stderr (2) -- three sources of stream. use `<` or `>` or `>>` to transfer stream into them

## chapter 4 Peek at some more advanced topics
- `df -h` -- to know the disk info
- some other command to know the version of the system, etc
- `apt-get upgrade` and some other commands


