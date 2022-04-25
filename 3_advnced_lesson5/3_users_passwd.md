cat /etc/passwd

login
root toor
exit

root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin

backdoor vulnerability:
assiging a user with 0 id makes him root - hard to detect...

useradd -m username -s /bin/bash
passwd username // assign pass to user

passwd -d user // no pass

תצורו את המשתמש helpdesk ואל תשכחו להגדיר למשתמש תיקיית בית.
2 .הכניסו את המשתמש לקבוצת sudo.
3 .בצעו את הפקודה
sudo vi /etc/passwd
4 .שנו את ה-id של המשתמש helpdesk ל-0 והתחברו למשתמש

useradd -m helpdesk -d /helpdesk -s /bin/bash
adduser helpdesk sudo
sudo vi /etc/passwd

useradd -m user1 -d /user1 -s /bin/bash; passwd -d user1
useradd -m user2 -d /user2 -s /bin/bash; passwd -d user2
useradd -m user3 -d /user3 -s /bin/bash; passwd -d user3

# assign user to groups
add user2 to user1 group
adduser user2 user1

mkdir /tmp/user_folder
<!-- change permissions so that:
only user1 group can enter this folder
--- --- ---
u   g   o
x - enter folder -->
chmod u=x , g=x , o= user_folder


can user2 create or view files in that folder: no.
can user3 create or view files in that folder: no.

can user2+3 enter folder - no (only 2)

5 .שנו את ההרשאות לתיקייה folder_user כך ש-user2 ו-user3 יוכלו לקרוא, ליצור ולהיכנס לתיקייה ו-
user1 לא יוכל לא להיכנס לתייקה, לא לצפות בתוכן שלה ולא ליצור קבצים.

chmod u=, g= , o=rxw user_folder

kick out user2 from user1 group...
deluser user2 user1 (:

