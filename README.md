# Learn-basic-linux-commands
Hello everyone, If you are interested in learning some basic Linux commands, so stick around. <br>
## 1-Lesson-Essential Elements:

1: <b>< cal ></b> This command is used for calender.
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

2: <b> < df -h > </b>  This command is same to up one but it will show the command in the human senseble.
##### For exmaple:
<per> muhiamen@sysbox:~/Data/cli-files-0.0$ df -h
Filesystem                 Size  Used Avail Use% Mounted on
udev                       1.8G     0  1.8G   0% /dev
tmpfs                      379M  1.7M  378M   1% /run
/dev/mapper/vgubuntu-root  291G   64G  212G  24% /
tmpfs                      1.9G     0  1.9G   0% /dev/shm
tmpfs                      5.0M  4.0K  5.0M   1% /run/lock
tmpfs                      1.9G     0  1.9G   0% /sys/fs/cgroup
/dev/loop0                 128K  128K     0 100% /snap/bare/5
/dev/loop1                 252M  252M     0 100% /snap/brave/135
/dev/loop3                  56M   56M     0 100% /snap/core18/2128
/dev/loop7                  66M   66M     0 100% /snap/gtk-common-themes/1519
/dev/loop6                 219M  219M     0 100% /snap/gnome-3-34-1804/72
/dev/loop5                 256M  256M     0 100% /snap/gnome-3-34-1804/36
/dev/loop9                  50M   50M     0 100% /snap/snap-store/467
/dev/loop4                  56M   56M     0 100% /snap/core18/2246
/dev/loop8                  63M   63M     0 100% /snap/gtk-common-themes/1506
/dev/loop2                 252M  252M     0 100% /snap/brave/134
/dev/loop10                 51M   51M     0 100% /snap/snap-store/547
/dev/loop11                 33M   33M     0 100% /snap/snapd/13640
/dev/loop12                 33M   33M     0 100% /snap/snapd/13270
/dev/loop14                2.2M  2.2M     0 100% /snap/utorrent/97
/dev/loop13                347M  347M     0 100% /snap/wine-platform-runtime/254
/dev/loop15                100M  100M     0 100% /snap/wine-platform-3-stable/14
/dev/loop16                347M  347M     0 100% /snap/wine-platform-runtime/267
/dev/sda2                  705M  329M  326M  51% /boot
/dev/sda1                  511M  5.3M  506M   2% /boot/efi
tmpfs                      379M   40K  379M   1% /run/user/1000 </pre>
  
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
I am doning partice of command line
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
root          10  0.0  0.0      0     0 ?        S    10:00   0:00 [rcu_tasks_tr
root          11  0.0  0.0      0     0 ?        S    10:00   0:00 [ksoftirqd/0]
root          12  0.0  0.0      0     0 ?        I    10:00   0:04 [rcu_sched]
root          13  0.0  0.0      0     0 ?        S    10:00   0:00 [migration/0]
root          14  0.0  0.0      0     0 ?        S    10:00   0:00 [idle_inject/
root          15  0.1  0.0      0     0 ?        I    10:00   0:08 [kworker/0:1-
root          16  0.0  0.0      0     0 ?        S    10:00   0:00 [cpuhp/0]
root          17  0.0  0.0      0     0 ?        S    10:00   0:00 [cpuhp/1]
root          18  0.0  0.0      0     0 ?        S    10:00   0:00 [idle_inject/
root          19  0.0  0.0      0     0 ?        S    10:00   0:00 [migration/1]
root          20  0.0  0.0      0     0 ?        S    10:00   0:00 [ksoftirqd/1]
root          22  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/1:0H
root          23  0.0  0.0      0     0 ?        S    10:00   0:00 [cpuhp/2]
root          24  0.0  0.0      0     0 ?        S    10:00   0:00 [idle_inject/
root          25  0.0  0.0      0     0 ?        S    10:00   0:00 [migration/2]
root          26  0.0  0.0      0     0 ?        S    10:00   0:00 [ksoftirqd/2]
root          28  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/2:0H
root          29  0.0  0.0      0     0 ?        S    10:00   0:00 [cpuhp/3]
root          30  0.0  0.0      0     0 ?        S    10:00   0:00 [idle_inject/
root          31  0.0  0.0      0     0 ?        S    10:00   0:00 [migration/3]
root          32  0.0  0.0      0     0 ?        S    10:00   0:00 [ksoftirqd/3]
root          34  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/3:0H
root          35  0.0  0.0      0     0 ?        S    10:00   0:00 [kdevtmpfs]
root          36  0.0  0.0      0     0 ?        I<   10:00   0:00 [netns]
root          37  0.0  0.0      0     0 ?        I<   10:00   0:00 [inet_frag_wq
root          38  0.0  0.0      0     0 ?        S    10:00   0:00 [kauditd]
root          39  0.0  0.0      0     0 ?        S    10:00   0:00 [khungtaskd]
root          40  0.0  0.0      0     0 ?        S    10:00   0:00 [oom_reaper]
root          41  0.0  0.0      0     0 ?        I<   10:00   0:00 [writeback]
root          42  0.0  0.0      0     0 ?        S    10:00   0:00 [kcompactd0]
root          43  0.0  0.0      0     0 ?        SN   10:00   0:00 [ksmd]
root          44  0.0  0.0      0     0 ?        SN   10:00   0:00 [khugepaged]
root          91  0.0  0.0      0     0 ?        I<   10:00   0:00 [kintegrityd]
root          92  0.0  0.0      0     0 ?        I<   10:00   0:00 [kblockd]
root          93  0.0  0.0      0     0 ?        I<   10:00   0:00 [blkcg_punt_b
root          95  0.0  0.0      0     0 ?        I<   10:00   0:00 [tpm_dev_wq]
root          96  0.0  0.0      0     0 ?        I<   10:00   0:00 [ata_sff]
root          97  0.0  0.0      0     0 ?        I<   10:00   0:00 [md]
root          98  0.0  0.0      0     0 ?        I<   10:00   0:00 [edac-poller]
root          99  0.0  0.0      0     0 ?        I<   10:00   0:00 [devfreq_wq]
root         100  0.0  0.0      0     0 ?        S    10:00   0:00 [watchdogd]
root         102  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/0:1H
root         105  0.0  0.0      0     0 ?        S    10:00   0:00 [kswapd0]
root         106  0.0  0.0      0     0 ?        S    10:00   0:00 [ecryptfs-kth
root         108  0.0  0.0      0     0 ?        I<   10:00   0:00 [kthrotld]
root         109  0.0  0.0      0     0 ?        I<   10:00   0:00 [acpi_thermal
root         111  0.0  0.0      0     0 ?        I<   10:00   0:00 [vfio-irqfd-c
root         115  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/2:1H
root         116  0.0  0.0      0     0 ?        I<   10:00   0:00 [ipv6_addrcon
root         126  0.0  0.0      0     0 ?        I<   10:00   0:00 [kstrp]
root         129  0.0  0.0      0     0 ?        I<   10:00   0:00 [zswap-shrink
root         130  0.1  0.0      0     0 ?        I<   10:00   0:08 [kworker/u17:
root         137  0.0  0.0      0     0 ?        I<   10:00   0:00 [charger_mana
root         187  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/3:1H
root         189  0.0  0.0      0     0 ?        I<   10:00   0:00 [cryptd]
root         195  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_0]
root         196  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_0]
root         197  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_1]
root         198  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_1]
root         199  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_2]
root         200  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_2]
root         201  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_3]
root         202  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_3]
root         203  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_4]
root         204  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_4]
root         205  0.0  0.0      0     0 ?        S    10:00   0:00 [scsi_eh_5]
root         206  0.0  0.0      0     0 ?        I<   10:00   0:00 [scsi_tmf_5]
root         211  0.0  0.0      0     0 ?        I<   10:00   0:00 [kworker/1:1H
root         212  0.0  0.0      0     0 ?        S    10:00   0:00 [card0-crtc0]
root         213  0.0  0.0      0     0 ?        S    10:00   0:00 [card0-crtc1]
root         214  0.0  0.0      0     0 ?        S    10:00   0:00 [card0-crtc2]
root         533  0.0  0.0      0     0 ?        I<   10:00   0:00 [kdmflush]
root         546  0.0  0.0      0     0 ?        I<   10:00   0:00 [kcryptd_io/2
root         547  0.0  0.0      0     0 ?        I<   10:00   0:00 [kcryptd/253:
root         548  0.0  0.0      0     0 ?        S    10:00   0:00 [dmcrypt_writ
root         551  0.0  0.0      0     0 ?        I<   10:00   0:00 [kdmflush]
root         553  0.0  0.0      0     0 ?        I<   10:00   0:00 [kdmflush]
root         595  0.0  0.0      0     0 ?        S    10:00   0:00 [jbd2/dm-1-8]
root         596  0.0  0.0      0     0 ?        I<   10:00   0:00 [ext4-rsv-con
root         646  0.0  1.2  86040 46700 ?        S<s  10:01   0:00 /lib/systemd/
root         680  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop0]
root         682  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop1]
root         683  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop2]
root         685  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop3]
root         687  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop4]
root         688  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop5]
root         691  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop6]
root         693  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop7]
root         695  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop8]
root         696  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop9]
root         701  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop10]
root         705  0.0  0.2  24732  8196 ?        Ss   10:01   0:01 /lib/systemd/
root         706  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop11]
root         707  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop12]
root         708  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop13]
root         709  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop14]
root         710  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop15]
root         711  0.0  0.0      0     0 ?        S<   10:01   0:00 [loop16]
root         786  0.0  0.0      0     0 ?        S    10:01   0:00 [irq/32-mei_m
root         851  0.0  0.0      0     0 ?        I<   10:01   0:00 [cfg80211]
root         852  0.0  0.0      0     0 ?        S    10:01   0:00 [pccardd]
root        1028  0.0  0.0      0     0 ?        S    10:01   0:00 [jbd2/sda2-8]
root        1029  0.0  0.0      0     0 ?        I<   10:01   0:00 [ext4-rsv-con
systemd+    1078  0.0  0.3  24300 13584 ?        Ss   10:01   0:00 /lib/systemd/
root        1081  0.0  0.1 238716  7500 ?        Ssl  10:01   0:00 /usr/lib/acco
root        1082  0.0  0.0   2548   712 ?        Ss   10:01   0:01 /usr/sbin/acp
avahi       1085  0.0  0.0   8536  3292 ?        Ss   10:01   0:00 avahi-daemon:
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
root        1242  0.0  0.0      0     0 ?        S    10:01   0:00 [ath9k-hwrng]
whoopsie    1309  0.0  0.3 326864 15180 ?        Ssl  10:01   0:00 /usr/bin/whoo
kernoops    1317  0.0  0.0  11264   444 ?        Ss   10:01   0:00 /usr/sbin/ker
kernoops    1319  0.0  0.0  11264   448 ?        Ss   10:01   0:00 /usr/sbin/ker
root        1343  0.0  0.0      0     0 ?        I<   10:01   0:00 [iprt-VBoxWQu
root        1344  0.0  0.0      0     0 ?        S    10:01   0:00 [iprt-VBoxTsc
rtkit       1366  0.0  0.0 152940  2972 ?        SNsl 10:02   0:00 /usr/libexec/
root        1468  0.0  0.2 252760 10128 ?        Ssl  10:02   0:00 /usr/lib/upow
root        1687  0.0  0.0      0     0 ?        I<   10:02   0:00 [kworker/u17:
root        1693  0.0  0.2 167532  9564 ?        Sl   10:02   0:00 gdm-session-w
muhiamen    1708  0.0  0.2  19200 10400 ?        Ss   10:02   0:00 /lib/systemd/
muhiamen    1709  0.0  0.0 169064  3100 ?        S    10:02   0:00 (sd-pam)
muhiamen    1715  1.6  0.5 3245148 21148 ?       S<sl 10:02   1:42 /usr/bin/puls
muhiamen    1717  0.0  0.6 511844 24772 ?        SNsl 10:02   0:00 /usr/libexec/
muhiamen    1719  0.0  0.1   8672  5660 ?        Ss   10:02   0:01 /usr/bin/dbus
muhiamen    1736  0.0  0.2 240052  7924 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1741  0.0  0.1 378344  6504 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    1747  0.0  0.2 314404  9560 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1754  0.0  0.1 238444  7196 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1758  0.0  0.1 236212  5912 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1762  0.0  0.9 547540 36684 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    1769  0.0  0.2 315092  8928 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    1774  0.0  0.2 317060  8804 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1780  0.0  0.1 236040  5996 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1786  0.0  0.1 240496  7472 ?        Sl   10:02   0:00 /usr/bin/gnom
muhiamen    1807  0.0  0.1 164356  6620 tty2     Ssl+ 10:02   0:00 /usr/lib/gdm3
muhiamen    1809  4.8  1.6 819296 62908 tty2     Sl+  10:02   5:02 /usr/lib/xorg
colord      1847  0.0  0.3 246548 14408 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    1912  0.0  0.3 188560 13744 tty2     Sl+  10:02   0:00 /usr/libexec/
muhiamen    1985  0.0  0.0   6040   456 ?        Ss   10:02   0:00 /usr/bin/ssh-
muhiamen    2007  0.0  0.1 305424  6724 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2012  0.0  0.1   7248  4076 ?        S    10:02   0:00 /usr/bin/dbus
muhiamen    2022  0.0  0.1  90400  4344 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2029  0.0  0.4 558208 15688 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2043  3.6  5.8 4205368 227476 ?      Ssl  10:02   3:46 /usr/bin/gnom
muhiamen    2067  0.0  0.2 384976  8240 ?        Sl   10:02   0:00 ibus-daemon -
muhiamen    2071  0.0  0.1 236872  7128 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2072  0.0  0.8 275992 31620 ?        Sl   10:02   0:01 /usr/libexec/
muhiamen    2076  0.0  0.7 198188 28196 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2079  0.0  0.1 236840  7072 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2089  0.0  0.1 162876  7620 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2095  0.0  0.4 580992 18848 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2096  0.0  0.1 235936  4888 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2107  0.0  0.6 808400 25436 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2115  0.0  0.6 2660304 26296 ?       Sl   10:02   0:00 /usr/bin/gjs 
muhiamen    2126  0.0  0.1 310008  6516 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2127  0.0  0.7 578636 30104 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2128  0.0  0.4 373964 16096 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2130  0.0  0.2 312332  7876 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2132  0.0  0.7 346172 28336 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2133  0.0  0.8 688420 31364 ?        Ssl  10:02   0:01 /usr/libexec/
muhiamen    2134  0.0  0.7 687152 30840 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2139  0.0  0.2 248556 11288 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2142  0.0  0.1 457436  6024 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2146  0.0  0.1 235976  5980 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2149  0.0  0.2 465116  9960 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2153  0.0  0.2 315504  8184 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2154  0.0  0.2 319696  9092 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2162  0.0  0.1 385304  7116 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2164  0.0  0.7 271960 28088 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2167  0.0  0.2 314360  8152 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2169  0.0  0.7 346868 29556 ?        Ssl  10:02   0:00 /usr/libexec/
muhiamen    2189  0.0  1.5 639960 60844 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2193  0.0  0.1 231800  6068 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2225  0.0  0.3 342528 14848 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2243  0.0  0.1 163032  7024 ?        Sl   10:02   0:00 /usr/libexec/
muhiamen    2260  0.0  1.6 1114508 63616 ?       Sl   10:02   0:04 /snap/snap-st
muhiamen    2292  0.0  0.2 314292  8152 ?        Sl   10:03   0:00 /usr/libexec/
muhiamen    2293  0.0  0.1 531728  6448 ?        Ssl  10:03   0:00 /usr/libexec/
muhiamen    2312  0.0  0.7 1117572 29928 ?       Ssl  10:03   0:00 /usr/libexec/
muhiamen    2358  0.0  0.1 156364  6008 ?        Sl   10:03   0:00 /usr/libexec/
muhiamen    2367  0.0  0.7 747264 29596 ?        Ssl  10:03   0:00 /usr/libexec/
muhiamen    2446  0.0  0.2 536660 10480 ?        Ssl  10:03   0:00 /usr/libexec/
muhiamen    2450  0.0  0.7 494004 28412 ?        Ssl  10:03   0:00 /usr/libexec/
root        2461  0.0  0.7 385264 28864 ?        Ssl  10:03   0:00 /usr/libexec/
muhiamen    2926  0.3  2.5 1151376 97452 ?       Sl   10:03   0:20 /usr/bin/naut
muhiamen    2978  0.0  0.1 162688  6456 ?        Ssl  10:03   0:00 /usr/libexec/
muhiamen    2981  0.0  0.7 493376 28896 ?        Sl   10:03   0:00 update-notifi
muhiamen    3412  7.6 14.3 4093232 558368 ?      Sl   10:46   4:38 /usr/lib/fire
muhiamen    3480  0.0  0.9 190512 38508 ?        Sl   10:46   0:00 /usr/lib/fire
muhiamen    3518  0.1  2.9 2421976 115836 ?      Sl   10:46   0:05 /usr/lib/fire
muhiamen    3569  2.9  4.4 2479580 173388 ?      Sl   10:46   1:47 /usr/lib/fire
muhiamen    3597  0.0  2.9 2437292 113164 ?      Sl   10:46   0:03 /usr/lib/fire
muhiamen    3829  0.8  2.3 884156 90540 ?        Sl   10:50   0:28 eog /home/muh
muhiamen    3864  0.5  1.3 816208 52788 ?        Ssl  10:52   0:17 /usr/libexec/
muhiamen    3872  0.0  0.1  11348  5600 pts/0    Ss   10:52   0:00 bash
muhiamen    4009  0.7  1.1 241360 45584 ?        Sl   10:56   0:22 /usr/lib/fire
muhiamen    4506  0.0  0.2 388184  8584 ?        Sl   10:58   0:00 /usr/libexec/
muhiamen    4524  0.0  0.2 315324  8228 ?        Sl   10:58   0:00 /usr/libexec/
root        4554  0.0  0.0      0     0 ?        I    11:00   0:01 [kworker/u16:
root        4582  0.1  0.0      0     0 ?        I    11:01   0:04 [kworker/2:2-
root        4657  0.0  0.0      0     0 ?        I    11:14   0:00 [kworker/u16:
root        4708  0.1  0.0      0     0 ?        I    11:19   0:01 [kworker/1:0-
root        4754  0.0  0.0      0     0 ?        I    11:24   0:00 [kworker/u16:
muhiamen    4861  0.0  0.1 360064  5684 ?        Sl   11:31   0:00 /usr/lib/spee
muhiamen    4864  0.0  0.2 450712  8184 ?        Sl   11:31   0:00 /usr/lib/spee
muhiamen    4870  0.0  0.0 160072  2360 ?        Ssl  11:31   0:00 /usr/bin/spee
root        4883  0.0  0.0      0     0 ?        I    11:31   0:00 [kworker/u16:
root        4901  0.1  0.0      0     0 ?        I    11:32   0:00 [kworker/3:2-
root        4963  0.0  0.0      0     0 ?        I    11:37   0:00 [kworker/u16:
root        4965  0.0  0.0      0     0 ?        I    11:38   0:00 [kworker/3:1-
root        4966  0.0  0.0      0     0 ?        I    11:38   0:00 [kworker/1:2-
muhiamen    5010  2.3  3.8 2499812 147728 ?      Sl   11:39   0:09 /usr/lib/fire
root        5031  0.0  0.0      0     0 ?        I    11:39   0:00 [kworker/0:0-
root        5033  0.3  0.0      0     0 ?        I    11:40   0:01 [kworker/2:1-
muhiamen    5056  0.0  1.8 2381660 71996 ?       Sl   11:41   0:00 /usr/lib/fire
muhiamen    5110  0.0  0.0  11836  3416 pts/0    R+   11:46   0:00 ps aux
</pre>
  
3: 
  
  
  
  
  
  
  
  
  
  
  
  

  
  
  
  
  
  
  
