find /root/ -name "*.py"
find -name "f*0"

find -name passwd -ls

find / -size +150M 2>/dev/null

find . -type f //file
find . -type d // directory
find / -type l // link

+ display file name
/ display "solo" output

find / -name "passwd" -type f -exec grep secret {} \; 
cd ~


excercise:
lookup for a file "services" don't display errors in stdout but inside the service locate the ftp address

find / -name "services" -type f -exec grep ftp 2>/dev/null