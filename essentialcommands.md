#Essential Commands – 25% (https://www.youtube.com/watch?v=_2XU6__I944) 1:23:47
----type---
This shows if shell build in or provided by package

Ex : type cd, type less

Change HostName -centos
Super user
su
modfiy following
vi /etc/syscofig/network --HostName fqdn
vi /etc/hosts
restart network
/etc/init.d/network restart

---Ubuntu
su
vi /etc/sysctl.conf


//Find commmand
find . -name -name <filename>
find path -name -name <filename>
  
find empty files
find /tmp -type f -empty
  
//Archiving and Compression
tar czf myfiles.tar.gz file[1-5]
tar cjf myfiles.tar.bz2 file[1-5]
tar cJf myfiles.tar.xz file[1-5]
  
//to see inside
tar tvf myfiles.tar.gz
  
 
gzip -d myfiles.tar.gz
bzip2 -d myfiles.tar.bz2
xz -d myfiles.tar.xz
  
Extract 
tar xvf myfiles.tar
  
  
 //compressionn benchmark (https://www.rootusers.com/gzip-vs-bzip2-vs-xz-performance-comparison/)
  If you are interactively compressing files on the fly then you may want to do this quickly with gzip -6 (default compression level) or xz -1, 
  however if you’re configuring log rotation which will run automatically over night during a low resource usage period then it may be acceptable to use more CPU resources with xz -9 to save the greatest amount of space possible.
  For instance kernel.org compress the Linux kernel with xz, in this case spending extra time to compress the file well once makes sense when it will be downloaded and
  decompressed thousands of times resulting in bandwidth savings yet still decent decompression speeds.
  
  Stream
  Override operators sdin, sdout, sderr(2)
  >,<,2>
  Append operators
  >>,<<,2>>  
  
  Pipe operator (from getting output from one program to another )
  |
  Filters
  find,grep, tee, tr, wc
  
  
  
