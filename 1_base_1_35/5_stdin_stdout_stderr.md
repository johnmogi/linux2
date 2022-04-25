# comment a command
0 - stdin
1- stdout
2 - stderr

ls john 2> output
\\ היות שאין לי קובץ בשם זה תיווצר שגיאה, שים את תוכן השגיאה בקובץ
ls output 1> john
אם הקובץ אאוטפוט נמצא, שים את התכון בקובץ ג'ון

ls johnny >> result.txt 2>>error.txt
ls johnny >> result.txt 2>>&1
כאן בעצם ביקשתי שגם במקרה של טעות לשלוח את התוכן לקובץ

יש לזה קיצור דרך
ls johnny &> results.txt

grep johnny 2> /dev/null
לזרוק את הפקודה לסל המחזור בלי להציג את האאוטפוט בשום מקום.

EXCERCISE :
1. Ifconfig print only your ip
ifconfig | grep 'inet '
ifconfig | grep 'broadcast' | cut -d " " -f 10

2. find all "messages" move success to success.log and errors to error.log
find / -name 'messages' 1>success.log 2>error.log

3. same excercise as 2 but display in terminal only the successfull messages, do not display errors in stdout
find / -name 'messages'| tee 2>/dev/null

4. cut /etc/passwd but display each user on its own line
cut -d ":" 1 -f /etc/passwd
cut -d ":" 1 -f /etc/passwd | xargs echo

ifconfig | 10 / inet ?
