movie 25
## is there a way to retrieve course files?

() - define pattern as a group \\ בנוסף שרשור תבניות
{} number of appearences
[] number of options for a single char
. any char (similar to ? wildcard)
* the previous char appears 0 to any times
+  the previous char appears 1 to any times
^ begins in a given char 
$ ends in a given char

grep -Ernio "([1-9]{1,3}\.){3}[0-9]{1,3}" output

הצג תיקיות בלבד
ls -l | egrep ^d

EXCERCISE

1. display all ip's in /var/log/messages, save them into tmp/ip_log
cat /var/log/messages > /tmp/ip_log

2. display all files in folder using grep + ls
ls -l | grep ^-
egrep -nio "[0-9]{1}" log_ip
3. display all MAC adresses in the message file
3D:F2:C9:A6:B3:4F

4. display all lines with error or Error in messages also the line number

grep -nio "error" log_ip

>
