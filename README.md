# Learn-basic-linux-commands
Hello everyone, If you are interested in learning some basic Linux commands, so stick around here. <br>

# summary:
In this course we are going to cover the following commands line: <br>
In <b> 1-lesson </b> : <br> 
<pre> cal, date. </pre>
In <b> 2-lesson </b> : <br>
<pre> ls, cd, cd .. </pre>
In <b> 3-lesson </b> : <br>
<pre> pwd, touch, cat, wc. </pre>
In <b> 4-lesson </b> : <br>
<pre> info, whatis, man. </pre>
In <b> 5-lesson </b> : <br>
<pre> grep, mv, rm, cp, rmdir. </pre>
In <b> 6-lesson </b> : <br>
<pre> df, df -h, du, du -h, du -sh*, find, tail, echo, top. </pre>
In <b> 7-lesson </b> : <br>
<pre> ps u, ps aux, ps aux | grep *, kill, cat /proc/cpuinfo, cat /proc/meminfo, ifconfig, mslookup *. </pre>
In <b> 8-lesson </b> : <br>
<pre> ctrl+r, history, apt-get, passwd, poweroff. </pre>

<br>

# Lessons:
## 1-Lesson-Essential Elements:

1: <b>< cal ></b> This command is used for calendar.
##### For example:
<pre>muhaimen@sysbox:~$ cal <br>
  November 2021      
Su Mo Tu We Th Fr Sa  
    1  2  3  4  5  6  
 7  8  9 10 11 12 13  
14 15 16 17 18 19 20  
21 22 23 24 25 26 27  
28 29 30 <br><br></pre>

2: <b> < date > </b> This command is used for date.
##### For example:
<pre>muhiamen@sysbox:~$ date <br>
Sun  7 Nov 20:58:13 PKT 2021</pre>
  
## 2-Lesson-Working with directories:

1:<b> < mkdir > </b> Through this command we can make directory.<br>
##### For Example:
<pre>muhiamen@sysbox:~$ mkdir Getting-start.<br></pre> 
<i> Then again shell will came without any error so it mean that directory is made.</i> <br>

2: <b> < ls > </b> This command is used for list mean to know about the items in the directoy.<b
##### For Example:
muhiamen@sysbox:~$ ls <br><pre>
'Books for study'           My-data<br>
 Music                      Pictures<br>
 Desktop                    New<br>
 Document                   Public<br>
 Getting-start              Download<br>
 Movies                     Videos<br>
 </pre> <br>
 
  
3: <b> < cd > </b> Through this command you can enter into the directory or folder.
##### For Example:
 <pre>  muhiamen@sysbox:~$ cd Getting-start <br>
   muhiamen@sysbox:~/Getting-start$</pre>

4: <b> < cd .. > </b> Trough this command you can go out from the directory or folder.
##### For example:
<pre> muhiamen@sysbox:~/Getting-start$ cd ..
muhiamen@sysbox:~$ </pre>


## 3-Lesson-Working with Files:

  1: <b> < pwd > </b> This command shows us the Present Working Directory.
  ##### For Example:
  <pre>muhiamen@sysbox:~/Getting-start$ pwd <br>
/home/muhiamen/Getting-start</pre>
  
  2: <b> < touch > </b> This command is used to make file.
  ##### For Example:
  <pre>muhiamen@sysbox:~/Getting-start$ touch hello.txt <br></pre>
  ###### Note: Again if the shell comes back with no error so it means that the files has been made.</i>
    
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
  ###### Note: If the their is no error so it means that the command has been worked.
 
  3: <b> < mv > </b> This command is used to move (rename) files.
  ##### For example:
 <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-03$ mv iris.backup.cv iris-folder/ </pre>
 ###### Note:If the command doesn't give any error so it means that it has worked correctly.
  
  4: <b> < rm > </b> This command is used to remove files or directories.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-03$ rm -r iris-folder.1 </pre>
  ###### Note: Again if their is no error so it means that the command has worked properly.
  
  5: <b> < cp > </b> This command is used to copy files and directories.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-03$ cp -r backup backup-2 </pre>
  
  6: <b> < rmdir > </b> This command is aslo used to remove files or directories.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0/lesson-03$ rmdir remove </pre>
  ###### Note: Again if their is no error so it means that the command has worked properly.
  
  ## 6-Lesson:
  1: <b> < df > </b> This command is used to report file system disk space usage.
  ##### For example:
  <pre> muhiamen@sysbox:~/Data/cli-files-0.0$ df
Filesystem                1K-blocks     Used Available Use% Mounted on
udev                        1886740        0   1886740   0% /dev
tmpfs                        387900     1680    386220   1% /run
/dev/mapper/vgubuntu-root 304309384 66938432 221843224  24% /
tmpfs                       1939480        0   1939480   0% /dev/shm
tmpfs                          5120        4      5116   1% /run/lock
tmpfs                       1939480        0   1939480   0% /sys/fs/cgroup
/dev/loop0                      128      128         0 100% /snap/bare/5
/dev/loop1                   257408   257408         0 100% /snap/brave/135
/dev/loop3                    56832    56832         0 100% /snap/core18/2128
/dev/loop7                    66816    66816         0 100% /snap/gtk-common-themes/1519
/dev/loop6                   224256   224256         0 100% /snap/gnome-3-34-1804/72
/dev/loop5                   261760   261760         0 100% /snap/gnome-3-34-1804/36
/dev/loop9                    51072    51072         0 100% /snap/snap-store/467
/dev/loop4                    56832    56832         0 100% /snap/core18/2246
/dev/loop8                    63616    63616         0 100% /snap/gtk-common-themes/1506
/dev/loop2                   257408   257408         0 100% /snap/brave/134
/dev/loop10                   52224    52224         0 100% /snap/snap-store/547
/dev/loop11                   33280    33280         0 100% /snap/snapd/13640
/dev/loop12                   33280    33280         0 100% /snap/snapd/13270
/dev/loop14                    2176     2176         0 100% /snap/utorrent/97
/dev/loop13                  355328   355328         0 100% /snap/wine-platform-runtime/254
/dev/loop15                  101888   101888         0 100% /snap/wine-platform-3-stable/14
/dev/loop16                  355072   355072         0 100% /snap/wine-platform-runtime/267
/dev/sda2                    721392   336092    332836  51% /boot
/dev/sda1                    523248     5356    517892   2% /boot/efi
tmpfs                        387896       40    387856   1% /run/user/1000 </pre>


2: <b> < df -h > </b> This command is same to up one but it will show the command in the human senseble.
##### For exmaple:
<pre> muhiamen@sysbox:~$ df -h
Filesystem                 Size  Used Avail Use% Mounted on
udev                       1.8G     0  1.8G   0% /dev
tmpfs                      379M  1.7M  378M   1% /run
/dev/mapper/vgubuntu-root  291G   64G  212G  24% /
tmpfs                      1.9G   85M  1.8G   5% /dev/shm
tmpfs                      5.0M  4.0K  5.0M   1% /run/lock
tmpfs                      1.9G     0  1.9G   0% /sys/fs/cgroup
/dev/loop1                 252M  252M     0 100% /snap/brave/135
/dev/loop2                 128K  128K     0 100% /snap/bare/5
/dev/loop3                  56M   56M     0 100% /snap/core18/2128
/dev/loop0                 252M  252M     0 100% /snap/brave/134
/dev/loop5                 256M  256M     0 100% /snap/gnome-3-34-1804/36
/dev/loop4                  56M   56M     0 100% /snap/core18/2246
/dev/loop8                  63M   63M     0 100% /snap/gtk-common-themes/1506
/dev/loop6                 219M  219M     0 100% /snap/gnome-3-34-1804/72
/dev/loop7                  66M   66M     0 100% /snap/gtk-common-themes/1519
/dev/loop10                 33M   33M     0 100% /snap/snapd/13270
/dev/loop11                 51M   51M     0 100% /snap/snap-store/547
/dev/loop12                 33M   33M     0 100% /snap/snapd/13640
/dev/loop9                  50M   50M     0 100% /snap/snap-store/467
/dev/loop13                2.2M  2.2M     0 100% /snap/utorrent/97
/dev/loop14                347M  347M     0 100% /snap/wine-platform-runtime/267
/dev/loop15                347M  347M     0 100% /snap/wine-platform-runtime/254
/dev/loop16                100M  100M     0 100% /snap/wine-platform-3-stable/14
/dev/sda2                  705M  329M  326M  51% /boot
/dev/sda1                  511M  5.3M  506M   2% /boot/efi
tmpfs                      379M   36K  379M   1% /run/user/1000 </pre>


  
3: <b> < du > </b> This command is used to estimate file space usage.
##### For example:
<pre> muhiamen@sysbox:~/Data/cli-files-0.0$ du
4	./extras
4	./trying
4	./on
12	./lesson-03/iris-folder
4	./lesson-03/backup
20	./lesson-03
4	./cmd
8	./lesson-01
20	./lesson-04/iris-data
336	./lesson-04/housing-data
360	./lesson-04
12	./lesson-02
12	./lesson-05
444	. </pre>
  
4: <b> < du -h > </b>  This also same to df -h.
##### For example:
<pre> 4.0K	./extras
4.0K	./trying
4.0K	./on
12K	./lesson-03/iris-folder
4.0K	./lesson-03/backup
20K	./lesson-03
4.0K	./cmd
8.0K	./lesson-01
20K	./lesson-04/iris-data
336K	./lesson-04/housing-data
360K	./lesson-04
12K	./lesson-02
12K	./lesson-05
444K	. </pre>
 
  
5: <b> < du -sh * > Here the <b> -sh </b> mean to search.
##### For example:
<pre> muhiamen@sysbox:~/Data/cli-files-0.0$ du -sh *
4.0K	cmd
4.0K	extras
4.0K	hello.txt
8.0K	lesson-01
12K	lesson-02
20K	lesson-03
360K	lesson-04
12K	lesson-05
4.0K	on
4.0K	README.md
4.0K	temp1
4.0K	trying </pre>
  
6: <b> < find > </b> This command is used to search for files in a directory hierarchy.
##### For example:
<pre> muhiamen@sysbox:~/Data/cli-files-0.0$ find -name lesson-01
./lesson-0 </pre>

###### Note: After find you have to write about the <b> type </b>  and then name or size . 
  
7: <b> < tail * > </b> This command is used to output the last part of files.
##### For example:
<pre> muhiamen@sysbox:~/Data/cli-files-0.0$ tail hello.txt 
something </pre> 
  
8: <b> < echo > </b> This command is used to display a line of text.
##### For example:
<pre> muhiamen@sysbox:~/Data/cli-files-0.0$ echo "I am doning partice of command line"> hello.txt.
muhiamen@sysbox:~/Data/cli-files-0.0$ cat hello.txt 
I am doing practice of command line
muhiamen@sysbox:~/Data/cli-files-0.0$  </pre>

9:<b> < top > This command is used to display Linux processes
##### For example:
<pre>muhiamen@sysbox:~/Data/cli-files-0.0/lesson-01$ top

top - 11:31:58 up  1:31,  1 user,  load average: 1.21, 0.53, 0.42
Tasks: 242 total,   1 running, 241 sleeping,   0 stopped,   0 zombie
%Cpu(s): 10.8 us,  5.6 sy,  0.0 ni, 81.9 id,  1.4 wa,  0.0 hi,  0.3 si,  0.0 st
MiB Mem :   3788.1 total,    323.4 free,   1309.2 used,   2155.5 buff/cache
MiB Swap:    976.0 total,    975.0 free,      1.0 used.   1907.0 avail Mem 

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND  
   3412 muhiamen  20   0 3756232 508248 191584 S  30.2  13.1   3:37.10 GeckoMa+ 
   4139 muhiamen  20   0 2703816 215924 106692 S  11.3   5.6   0:18.14 Web Con+ 
   1715 muhiamen   9 -11 2720860  21148  16188 S  10.0   0.5   0:39.16 pulseau+ 
   2043 muhiamen  20   0 4205648 227504  82828 S   8.3   5.9   3:23.34 gnome-s+ 
   1809 muhiamen  20   0  818916  62176  34592 S   4.3   1.6   4:38.11 Xorg     
    118 root      20   0       0      0      0 I   0.7   0.0   0:11.16 kworker+ 
   1747 muhiamen  20   0  314404   9560   7764 S   0.7   0.2   0:00.44 gvfs-ud+ 
     15 root      20   0       0      0      0 I   0.3   0.0   0:07.32 kworker+ 
    130 root       0 -20       0      0      0 D   0.3   0.0   0:07.88 kworker+ 
   1111 root      20   0  393180  13648  10484 S   0.3   0.4   0:00.80 udisksd  
   4523 root      20   0       0      0      0 I   0.3   0.0   0:00.86 kworker+ 
   4554 root      20   0       0      0      0 I   0.3   0.0   0:00.70 kworker+ 
   4582 root      20   0       0      0      0 I   0.3   0.0   0:02.70 kworker+ 
   4681 root      20   0       0      0      0 I   0.3   0.0   0:00.75 kworker+ 
   4708 root      20   0       0      0      0 I   0.3   0.0   0:00.74 kworker+ 
   4754 root      20   0       0      0      0 I   0.3   0.0   0:00.17 kworker+ 
   4800 root      20   0       0      0      0 I   0.3   0.0   0:00.11 kworker+  </pre>
  
  
  ## 7-Lesson:
  
  1: <b> < ps u > </b> This is command is used to report a snapshot of the current processes. <b> < u > </b> stands for a user-oriented format that provides detailed information about the processes.
  ##### For example:
  <pre> muhiamen@sysbox:/home$ ps u
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
muhiamen    1807  0.0  0.1 164356  6620 tty2     Ssl+ 10:02   0:00 /usr/lib/gdm3
muhiamen    1809  5.0  1.6 818940 62332 tty2     Sl+  10:02   4:47 /usr/lib/xorg
muhiamen    1912  0.0  0.3 188560 13744 tty2     Sl+  10:02   0:00 /usr/libexec/
muhiamen    3872  0.0  0.1  11348  5600 pts/0    Ss   10:52   0:00 bash
muhiamen    4920  0.0  0.0  11836  3496 pts/0    R+   11:36   0:00 ps u </pre>

2: <b> < ps aux > </b> The ps aux command is a tool to monitor processes running on your Linux system.  
##### For example:
<pre> muhiamen@sysbox:/home$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.3 167780 11668 ?        Ss   10:00   0:02 /sbin/init sp
root           2  0.0  0.0      0     0 ?        S    10:00   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        I<   10:00   0:00 [rcu_gp]
root           4  0.0  0.0      0     0 ?        I<   10:00   0:00 [rcu_par_gp]
root           6  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/0:0H
root           8  0.0  0.0      0     0 ?        I<   10:00   0:00 [mm_percpu_wq
root           9  0.0  0.0      0     0 ?        S    10:00   0:00 [rcu_tasks_ru
root        1086  0.0  0.0   9756  2900 ?        Ss   10:01   0:00 /usr/sbin/cro
root        1087  0.0  0.2  28912  8908 ?        Ss   10:01   0:00 /usr/sbin/cup
message+    1088  0.0  0.1   9832  5928 ?        Ss   10:01   0:02 /usr/bin/dbus
root        1089  0.2  0.5 410392 20272 ?        Ssl  10:01   0:16 /usr/sbin/Net
root        1095  0.0  0.0  81904  3660 ?        Ssl  10:01   0:00 /usr/sbin/irq
root        1097  0.0  0.5  39668 20156 ?        Ss   10:01   0:00 /usr/bin/pyth
root        1100  0.0  0.2 235048  9632 ?        Ssl  10:01   0:02 /usr/lib/poli
syslog      1102  0.0  0.1 224532  4980 ?        Ssl  10:01   0:00 /usr/sbin/rsy
root        1105  0.0  0.7 1367276 29720 ?       Ssl  10:01   0:02 /usr/lib/snap
root        1106  0.0  0.1 235944  6112 ?        Ssl  10:01   0:00 /usr/libexec/
root        1109  0.0  0.2  16748  8352 ?        Ss   10:01   0:00 /lib/systemd/
root        1110  0.0  0.2 126612  9360 ?        Ssl  10:01   0:00 /usr/sbin/the
root        1111  0.0  0.3 393180 13648 ?        Ssl  10:01   0:00 /usr/lib/udis
root        1112  0.0  0.2  14088  8084 ?        Ss   10:01   0:00 /sbin/wpa_sup
avahi       1139  0.0  0.0   8352   328 ?        S    10:01   0:00 avahi-daemon:
root        1188  0.0  0.3 178400 12608 ?        Ssl  10:01   0:00 /usr/sbin/cup
root        1193  0.0  0.5 118468 22840 ?        Ssl  10:01   0:00 /usr/bin/pyth
root        1204  0.0  0.2 240724 11044 ?        Ssl  10:01   0:00 /usr/sbin/Mod
root        1207  0.0  0.2 239952  8664 ?        Ssl  10:01   0:00 /usr/sbin/gdm
muhiamen    5110  0.0  0.0  11836  3416 pts/0    R+   11:46   0:00 ps aux
.......... </pre>
  
3: <b> < ps aux | grep * > </b> In this command you can search for match patterns of the current processe
##### For example:
 <pre> muhiamen@sysbox:~$ ps aux | grep firefox
muhiamen    3067 10.3  8.5 3275568 333392 pts/1  Sl+  17:08   1:28 /usr/lib/firefox/firefox
muhiamen    3132  0.0  1.0 190516 39208 pts/1    Sl+  17:08   0:00 /usr/lib/firefox/firefox -contentproc -parentBuildID 20211028161635 -prefsLen 1 -prefMapSize 243591 -appdir /usr/lib/firefox/browser 3067 true socket
muhiamen    3153  0.1  2.9 2423644 116368 pts/1  Sl+  17:08   0:01 /usr/lib/firefox/firefox -contentproc -childID 1 -isForBrowser -prefsLen 102 -prefMapSize 243591 -jsInit 278680 -parentBuildID 20211028161635 -appdir /usr/lib/firefox/browser 3067 true tab
muhiamen    3197  7.5  4.7 2483076 185344 pts/1  Sl+  17:08   1:04 /usr/lib/firefox/firefox -contentproc -childID 2 -isForBrowser -prefsLen 268 -prefMapSize 243591 -jsInit 278680 -parentBuildID 20211028161635 -appdir /usr/lib/firefox/browser 3067 true tab
muhiamen    3224  0.1  2.5 2424992 99932 pts/1   Sl+  17:08   0:01 /usr/lib/firefox/firefox -contentproc -childID 3 -isForBrowser -prefsLen 4880 -prefMapSize 243591 -jsInit 278680 -parentBuildID 20211028161635 -appdr /usr/lib/firefox/browser 3067 true tab
muhiamen    3264  0.0  1.8 2381132 72464 pts/1   Sl+  17:08   0:00 /usr/lib/firefox/firefox -contentproc -childID 4 -isForBrowser -prefsLen 5579 -prefMapSize 243591 -jsInit 278680 -parentBuildID 20211028161635 -appdir /usr/lib/firefox/browser 3067 true tab
muhiamen    4090  0.0  0.0   9380   736 pts/0    S+   17:22   0:00 grep --color=auto firefox
</pre>
  
4: <b> < kill > </b> This command is used to kill a current processe. But with near the muhaimen there is number which is 3067 in up example copy that number and put that number in the last of kill command. Like this <b> kill -9 3067 </b>
##### For example:
<pre> 
  
  
  
  
  
</pre>  
  
5: <b> < cat /proc/cpuinfo > </b> This command is used to to info about the cpu prosoccer.
##### For example:
<pre> muhiamen@sysbox:~$ cat /proc/cpuinfo
processor	: 0
vendor_id	: GenuineIntel
cpu family	: 6
model		: 58
model name	: Intel(R) Core(TM) i3-3110M CPU @ 2.40GHz
stepping	: 9
microcode	: 0x21
cpu MHz		: 1410.906
cache size	: 3072 KB
physical id	: 0
siblings	: 4
core id		: 0
cpu cores	: 2
apicid		: 0
initial apicid	: 0
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer xsave avx f16c lahf_lm cpuid_fault epb pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms xsaveopt dtherm arat pln pts md_clear flush_l1d
vmx flags	: vnmi preemption_timer invvpid ept_x_only flexpriority tsc_offset vtpr mtf vapic ept vpid unrestricted_guest
bugs		: cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit
bogomips	: 4788.97
clflush size	: 64
cache_alignment	: 64
address sizes	: 36 bits physical, 48 bits virtual
power management:

processor	: 1
vendor_id	: GenuineIntel
cpu family	: 6
model		: 58
model name	: Intel(R) Core(TM) i3-3110M CPU @ 2.40GHz
stepping	: 9
microcode	: 0x21
cpu MHz		: 1300.000
cache size	: 3072 KB
physical id	: 0
siblings	: 4
core id		: 0
cpu cores	: 2
apicid		: 1
initial apicid	: 1
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer xsave avx f16c lahf_lm cpuid_fault epb pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms xsaveopt dtherm arat pln pts md_clear flush_l1d
vmx flags	: vnmi preemption_timer invvpid ept_x_only flexpriority tsc_offset vtpr mtf vapic ept vpid unrestricted_guest
bugs		: cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit
bogomips	: 4788.97
clflush size	: 64
cache_alignment	: 64
address sizes	: 36 bits physical, 48 bits virtual
power management:

processor	: 2
vendor_id	: GenuineIntel
cpu family	: 6
model		: 58
model name	: Intel(R) Core(TM) i3-3110M CPU @ 2.40GHz
stepping	: 9
microcode	: 0x21
cpu MHz		: 1400.000
cache size	: 3072 KB
physical id	: 0
siblings	: 4
core id		: 1
cpu cores	: 2
apicid		: 2
initial apicid	: 2
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer xsave avx f16c lahf_lm cpuid_fault epb pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms xsaveopt dtherm arat pln pts md_clear flush_l1d
vmx flags	: vnmi preemption_timer invvpid ept_x_only flexpriority tsc_offset vtpr mtf vapic ept vpid unrestricted_guest
bugs		: cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit
bogomips	: 4788.97
clflush size	: 64
cache_alignment	: 64
address sizes	: 36 bits physical, 48 bits virtual
power management:

processor	: 3
vendor_id	: GenuineIntel
cpu family	: 6
model		: 58
model name	: Intel(R) Core(TM) i3-3110M CPU @ 2.40GHz
stepping	: 9
microcode	: 0x21
cpu MHz		: 1707.031
cache size	: 3072 KB
physical id	: 0
siblings	: 4
core id		: 1
cpu cores	: 2
apicid		: 3
initial apicid	: 3
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer xsave avx f16c lahf_lm cpuid_fault epb pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms xsaveopt dtherm arat pln pts md_clear flush_l1d
vmx flags	: vnmi preemption_timer invvpid ept_x_only flexpriority tsc_offset vtpr mtf vapic ept vpid unrestricted_guest
bugs		: cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit
bogomips	: 4788.97
clflush size	: 64
cache_alignment	: 64
address sizes	: 36 bits physical, 48 bits virtual
power management: </pre>
  
  
6: <b> < cat /proc/meminfo > </b> This command will show you detail about memory.
##### For example:
<pre> muhiamen@sysbox:~$ cat /proc/meminfo
MemTotal:        3878968 kB
MemFree:          319076 kB
MemAvailable:    1704064 kB
Buffers:           96016 kB
Cached:          1849676 kB
SwapCached:            0 kB
Active:           695104 kB
Inactive:        2204468 kB
Active(anon):       3368 kB
Inactive(anon):  1364816 kB
Active(file):     691736 kB
Inactive(file):   839652 kB
Unevictable:      360396 kB
Mlocked:              48 kB
SwapTotal:        999420 kB
SwapFree:         999420 kB
Dirty:               836 kB
Writeback:             0 kB
AnonPages:       1314332 kB
Mapped:           598860 kB
Shmem:            419524 kB
KReclaimable:     111616 kB
Slab:             201728 kB
SReclaimable:     111616 kB
SUnreclaim:        90112 kB
KernelStack:       13648 kB
PageTables:        27864 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     2938904 kB
Committed_AS:    7258836 kB
VmallocTotal:   34359738367 kB
VmallocUsed:       32844 kB
VmallocChunk:          0 kB
Percpu:             7744 kB
HardwareCorrupted:     0 kB
AnonHugePages:         0 kB
ShmemHugePages:        0 kB
ShmemPmdMapped:        0 kB
FileHugePages:         0 kB
FilePmdMapped:         0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
Hugetlb:               0 kB
DirectMap4k:      267188 kB
DirectMap2M:     3784704 kB </pre>
 
7: <b> < ifconfig > </b> This stands for Interface configuration. It's function is Configure network interface parameters.
##### For example:
<pre> muhiamen@sysbox:~$ ifconfig
enp3s0: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        ether e0:18:77:03:b6:0c  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 4479  bytes 395041 (395.0 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 4479  bytes 395041 (395.0 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

wlp4s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.43.60  netmask 255.255.255.0  broadcast 192.168.43.255
        inet6 fe80::7984:33d6:d68d:91f6  prefixlen 64  scopeid 0x20<link>
        ether c0:d9:62:82:86:39  txqueuelen 1000  (Ethernet)
        RX packets 77291  bytes 100582757 (100.5 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 39785  bytes 6131432 (6.1 MB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
</pre>


8: <b> < nslookup * > This command is is a network administration command-line tool for querying the Domain Name System to obtain the mapping between domain name and IP address, or other DNS records.
##### For example:
<pre> muhiamen@sysbox:~$ nslookup yahoo.com
Server:		127.0.0.53
Address:	127.0.0.53#53

Non-authoritative answer:
Name:	yahoo.com
Address: 74.6.231.20
Name:	yahoo.com
Address: 74.6.231.21
Name:	yahoo.com
Address: 98.137.11.164
Name:	yahoo.com
Address: 98.137.11.163
Name:	yahoo.com
Address: 74.6.143.25
Name:	yahoo.com
Address: 74.6.143.26
Name:	yahoo.com
Address: 2001:4998:124:1507::f000
Name:	yahoo.com
Address: 2001:4998:44:3507::8000
Name:	yahoo.com
Address: 2001:4998:24:120d::1:1
Name:	yahoo.com
Address: 2001:4998:124:1507::f001
Name:	yahoo.com
Address: 2001:4998:24:120d::1:0
Name:	yahoo.com
Address: 2001:4998:44:3507::8001 </pre>
</pre>
 
## 8-Lesson: 

1: <b> < ctrl+r > </b> This command is recall the last command matching the characters you provide.

2: <b> < history > </b> This command is used to show previously used commands or to
get information about the commands executed by a user.
##### For example:
<pre> muhiamen@sysbox:~$ history
    5  anaconda-navigator
    6  sudo anaconda-navigator
    7  conda
    8  sudo su
    9  cd /root/
   10  sudo cd /root/
   11  sudo su
   12  cd
   13  cd.
   14  cd..
   15  cd ..
   16  ls/
   17  ls/.
   18  jupyter notebook
   19  cd Downloads/
   20  ls
   21  sudo chown 777 Anaconda3-2021.05-Linux-x86_64.sh 
   22  ls
   23  sudo chown -R 777 Anaconda3-2021.05-Linux-x86_64.sh 
   24  ls
   25  bash Anaconda3-2021.05-Linux-x86_64.sh 
   26  source ~/.bashrc
   27  conda list
   28  jupyter notebook
   29  exit
   30  cd
   31  ls
   32  cd . downloads
   33  ls
   34  cd Downloads
   35  ls
   36  cd..
   37  cd ..
   38  ls
   39  help
   40  help name
   41  pwd info name
   42  pwd info
   43  pwd type name
   44  help pwd
   45  cd Downloads
   46  ls
   47  sudo apt 
   48  firefox
   49  exit
   50  help
</pre>

3: <b> < apt-get > </b> apt -get is a powerful and free front-end package manager for
Debian/Ubuntu systems. It is used to install new software
packages, remove available software packages, upgrade
existing software packages as well as upgrade the entire
operating system. apt – stands for advanced packaging tool.
##### For example:
<pre> muhiamen@sysbox:~$ sudo apt-get update
Reading package lists... Done
E: Could not get lock /var/lib/apt/lists/lock. It is held by process 3499 (packagekitd)
N: Be aware that removing the lock file is not a solution and may break your system.
E: Unable to lock directory /var/lib/apt/lists/ </pre>

4: <b> < passwd > </b> Thorugh this command you can change the passward.

5: <b> < poweroff > </b> This command is used to poweroff the system.
##### For example:
<pre> muhiamen@sysbox:~$ poweroff
      muhiamen@sysbox:~$ </pre>


##### Try to do practice because the practice makes the man perfect.


#### Now it's time to acknowledge <a href="https://www.udemy.com/course/linux-command-line-zero-to-expert/?couponCode=PAST-STUDENTS-21-J" >Recluze</a> for has astonishing efforts who made me able to share these commands with you all.

#### If you have any problem in above commands first search it in google but still you have problem then you can mail me on <a href = "mailto: amuhaiminshah@gmail.com">Send Email</a>.
