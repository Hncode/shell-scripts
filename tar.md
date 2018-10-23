## tar command
### 1. Create tar Archive File
#### tar -cvf dest_example.tar src_example/
  -c : create a new .tar archive file.<br/>
  -v : verbosely show the .tar file progress.<br/>
  -f : file name type of the arcive file. <br/>
  
### 2. Create tar.gz Archive File
#### tar cvfz dest_example.tar.gz src_example/
  -z : create gzip compress file.
  
### 3. Create tar.gz Archive File
#### tar cvfj dest_example.tar.bz2 src_example/
  -j : create bz2 compress file.
  
### 4. Untar tar Archive File
#### tar -xvf dest_example.tar
#### tar -xvf dest_example.tar -C /home/usr/dest_dir/
  -x : extract

### 5. Uncompress tar.gz Archive File
#### tar -xvf src_example.tar.gz
#### tar -xvf src_example.tar.gz -C /home/usr/dest_dir/

### 6. Uncompress tar.bz2 Archive File
#### tar -xvf src_example.tar.bz2
#### tar -xvf src_example.tar.bz2 -C /home/usr/dest_dir/

### 7. List Content of tar Archive File
#### tar -tvf src_example.tar
-t : list content.


### 8. List Content of tar.gz Archive File
#### tar -tvf src_example.tar.gz
-t : list content.


### 9. List Content of tar.bz2 Archive File
#### tar -tvf src_example.tar.bz2
-t : list content.

### 10. Untar Single file from tar File
#### tar -xvf dest_example.tar file_in_dest.txt
#### tar --extract --file=sripts.sh.tar sripts.sh

### 11. Untar Single file from tar.gz File
#### tar -zxvf dest_example.tar.gz file_in_dest.txt
#### tar --extract --file=sripts.sh.tar.gz sripts.sh

### 12. Untar Single file from tar.bz2 File
#### tar -jxvf dest_example.tar.bz2 file_in_dest.txt
#### tar --extract --file=sripts.sh.tar.bz2 sripts.sh
  
### 13. Untar Multiple files from tar, tar.gz and tar.bz2 File
#### tar -xvf tecmint-14-09-12.tar "file 1" "file 2"
#### tar -zxvf MyImages-14-09-12.tar.gz "file 1" "file 2"
#### tar -jxvf Phpfiles-org.tar.bz2 "file 1" "file 2"


### 14. Extract Group of Files using Wildcard
#### tar -xvf Phpfiles-org.tar --wildcards '*.php'
#### tar -zxvf Phpfiles-org.tar.gz --wildcards '*.php'
#### tar -jxvf Phpfiles-org.tar.bz2 --wildcards '*.php'

### 15. Add Files or Directories to tar Archive File
#### tar -rvf tecmint-14-09-12.tar xyz.txt
#### tar -rvf tecmint-14-09-12.tar dir

### 16. How To Verify tar, tar.gz and tar.bz2 Archive File
#### tar tvfW tecmint-14-09-12.tar

### 17. Check the Size of the tar, tar.gz and tar.bz2 Archive File
#### tar -czf - tecmint-14-09-12.tar | wc -c
#### tar -czf - MyImages-14-09-12.tar.gz | wc -c
#### tar -czf - Phpfiles-org.tar.bz2 | wc -c
