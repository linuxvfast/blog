
If you want to create a tar that contains only files specified in a file you can use the -T option.

**Example:**

    [bcane@bcane play]$ cat list.txt  
    1.txt  
    2.txt  
    3.txt  
    [bcane@bcane play]$ tar -cvzf files.tgz -T list.txt  
    1.txt  
    2.txt  
    3.txt  
    [bcane@bcane play]$ tar -tvzf files.tgz   
    -rw-rw-r-- bcane/bcane 0 2011-07-13 16:48 1.txt  
    -rw-rw-r-- bcane/bcane 0 2011-07-13 16:48 2.txt  
    -rw-rw-r-- bcane/bcane 0 2011-07-13 16:48 3.txt

-T will work for both creation and extraction of tar files.
