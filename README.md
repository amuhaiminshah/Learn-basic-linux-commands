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
  4: <b> < wc > </b> this command is used to print newline, word, and byte counts for each file. <br>
     #### For Example:
     <pre> muhiamen@sysbox:~/Data/cli-files-0.0$ wc hello.txt 
    1  1 10 hello.txt </pre>
  
  ## 4-Lesson-Need-Know-about-the-Command
