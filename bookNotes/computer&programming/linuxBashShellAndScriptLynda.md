# Linux bash Shell and Script

## chapter 1 Introduction to Bash Script
- `man` or `info` command or a reference mannual on the web -- help
- shebang `#!/bin/bash` -- to denote the bash used to run the script
- bash functions use braces and can modify variables of the shell that calls the function
- `source script` -- run the script in the current bash to introduce some variables ...
- `echo` to make the `\` to transform the character, you should use the quote mark and the `-e` option

## chapter 2 Variables, Control Structures and Arithmetic
- local variables
- `typeset`
- `declare`
- `read` to read one line of the file one time
- `while loop` or `for in loop`
- \`\` is to use the output of the command to alternate the parameters in the script; it is similar to the `$(command)` usage
- `seq 1 5` or `{A..Z}` to generate a sequence
- `return` & `exit` command; the exit status can be known using `echo $?`
- redirect things -- some useful messages and usages; be careful of the blank of words and the signs ==not quite understand it==
- case, ifThen, test command and some other test operators
- arithmetic operations with `(())`
- when using a `|`, it opens a new bash shell, so the while loop won't change the variables in teh previous shell; so you need to use the `>` to redirect the stream
 
## chapter 3 Using filters and parameter expansions
-`tail -n2 -f file` to echo the last two lines of the files and find if there are more lines exists, it is a way to read a constantly changing file 
- `awk` and `sed` -- some useful things ==i don't watch them carefully==
- positional strings with `{}` curly braces

== the note is stopped here, for i didn't need to use them, and the previous learning is just a brief contact with it. The bash is just a tool like pther programming languages, and don't immerse yourself into the language details. The idea is the most important==
