# Learn-basic-linux-commands
Hello everyone, If you are interested in learning some basic Linux commands, so stick around. <br>
## 1-Lesson-Essential Elements:

1: <b>< cal ></b> this command is used for calender.
##### For example:
<pre>muhaimen@sysbox:~$ cal <br>
  November 2021      
Su Mo Tu We Th Fr Sa  
    1  2  3  4  5  6  
 7  8  9 10 11 12 13  
14 15 16 17 18 19 20  
21 22 23 24 25 26 27  
28 29 30 <br><br></pre>

2: <b> < date > </b> this command is used for date.
##### For example:
<pre>muhiamen@sysbox:~$ date <br>
Sun  7 Nov 20:58:13 PKT 2021</pre>
  
## 2-Lesson-working with directories:

1:<b> < mkdir > </b> through this command we can make directory.<br>
##### For Example:
<pre>muhiamen@sysbox:~$ mkdir Getting-start.<br></pre> 
<i> Then again shell will came without any error so it mean that directory is made.</i> <br>

2: <b> < ls > </b> this command is used for list mean to know about the items in the directoy.<b
##### For Example:
muhiamen@sysbox:~$ ls <br><pre>
'Books for study'           My-data<br>
 Music                      Pictures<br>
 Desktop                    New<br>
 Document                   Public<br>
 Getting-start              Download<br>
 Movies                     Videos<br>
 </pre> <br>
 
  
3: <b> < cd > </b> through this command you can enter into the directory or folder.
##### For Example:
 <pre>  muhiamen@sysbox:~$ cd Getting-start <br>
   muhiamen@sysbox:~/Getting-start$</pre>

4: <b> < cd .. > </b> Trough this command you can go out from the directory or folder.
##### For example:
<pre> muhiamen@sysbox:~/Getting-start$ cd ..
muhiamen@sysbox:~$ </pre>


## 3-Lesson-Working with Files:

  1: <b> < pwd > </b> this command shows us the Present Working Directory.
  ##### For Example:
  <pre>muhiamen@sysbox:~/Getting-start$ pwd <br>
/home/muhiamen/Getting-start</pre>
  
  2: <b> < touch > </b> this command is used to make file.
  ##### For Example:
  <pre>muhiamen@sysbox:~/Getting-start$ touch hello.txt <br></pre>
  <i> again if the shell comes back with no error so it means that the files has been made.</i>
    
  3: <b> < cat > </b> this command concatenate files and print on the standard output.<br>
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0$ cat hello.txt 
    something</pre>
  4: <b> < wc > </b> this command is used to print newline, word, and byte counts for each file.
  #### For Example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0$ wc hello.txt 
    1  1 10 hello.txt </pre>
  
  ## 4-Lesson Need to Know more
  1: <b> < info > </b> First type info then type the name of the command.
  ##### For example:muhiamen@sysbox:~$ info wc
  <pre> Next: sum invocation,  Up: Summarizing files

6.1 ‘wc’: Print newline, word, and byte counts
==============================================

‘wc’ counts the number of bytes, characters, whitespace-separated words,
and newlines in each given FILE, or standard input if none are given or
for a FILE of ‘-’.  Synopsis:

     wc [OPTION]... [FILE]...

   ‘wc’ prints one line of counts for each file, and if the file was
given as an argument, it prints the file name following the counts.  If
more than one FILE is given, ‘wc’ prints a final line containing the
cumulative counts, with the file name ‘total’.  The counts are printed
in this order: newlines, words, characters, bytes, maximum line length.
Each count is printed right-justified in a field with at least one space
between fields so that the numbers and file names normally line up
nicely in columns.  The width of the count fields varies depending on
the inputs, so you should not depend on a particular field width.
However, as a GNU extension, if only one count is printed, it is
guaranteed to be printed without leading spaces.
-----Info: (coreutils)wc invocation, 83 lines --Top-----------------------------
Welcome to Info version 6.7.  Type H for help, h for tutorial. </pre>
  
2: <b> < whatis > </b> This also same to 1.
##### For example:
<pre> muhiamen@sysbox:~$ whatis wc
   wc (1)           - print newline, word, and byte counts for each file </pre>

3: <b> < man > </b> this will give you full detail about any command.
  ##### For example:
  <pre> muhiamen@sysbox:~$ man wc
  WC(1)                            User Commands                           WC(1)

NAME
       wc - print newline, word, and byte counts for each file

SYNOPSIS
       wc [OPTION]... [FILE]...
       wc [OPTION]... --files0-from=F

DESCRIPTION
       Print newline, word, and byte counts for each FILE, and a total line if
       more than one FILE is specified.  A word is a non-zero-length  sequence
       of characters delimited by white space.

       With no FILE, or when FILE is -, read standard input.

       The  options  below may be used to select which counts are printed, al‐
       ways in the following order: newline, word,  character,  byte,  maximum
       line length.

       -c, --bytes
              print the byte counts
 Manual page wc(1) line 1 (press h for help or q to quit) </pre>
  
 ## 5-Lesson:
  1: <b> < grep > </b> This command is used to print lines that match pattern.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-01$ cat dummy-file.txt | grep "test"
        I am a test file. </pre>
  2: <b> < mv > </b> This command is used to move (rename) files.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-03$ mv iris.csv iris.backup.cv </pre>
  If the their is no error so it means that the command has been worked.
 
