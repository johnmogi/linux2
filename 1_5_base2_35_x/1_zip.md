apt install zip

zip file.zip file1 file 2 *
zip -r backup.zip /root/prog/*
unzip


gzip file
gzip -c // שומר על המקור

vi file.gzip

gunzip file.gz // פתיחת קובץ דחוס

bzip2
bunzip2 -k

tar // יודעת גם לדחוס תיקיות

-c // compress
-x // extract
-v // display additional info during compression
-f // disply files (joined with v)
-z /// gzip
-j // bzip2
J // xz - lp101
-t // display tar without open
-C // choose where to extract


date +%y-%m-%d

echo  $(date +%y-%m-%d)
echo `date +%y-%m-%d`


excercise:

compress all files at root folder
name compressed file to:
backup_file_current_date
replace current_date with todays date
place compressed file at tmp


tar -zcvf /tmp/backup_file_$(date +%Y-%m-%d).tar.gz /root/*

tar -tvf backup_file_2021-12-09.tar.gz
