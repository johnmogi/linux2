~ \\תיקית הבית של היוזר
cd /var/www
cd ~
cd - \\ מחזיר אותי למקום הקודם בו הייתי

cd . \\ התיקייה הנוכחית - שימושי לקבצים
cd .. \\ תיקייה אחת למעלה

Tab - השלמה אוטומטית מתוך חלקי הפקודה
clear - ניקיון הלוח

גלגל עכבר - העתקת קבצים מהירה בטרמינל
cd ~
mkdir folder1
mv folder1 /tmp
cd tmp
mv folder1 new_folder \\ כאשר זה באותו מיקום פקודת מו משנה שם
cp העתקה
cp file new_file
cp file /var/www/

rm -r <folder> \\ רקורסיב למחוק את כל הקבצים
לא להשתמש ב F \\ FORCE
לא להשתמש ב \
rm -rf \ \\מחיקת כל הקבצים מהמחשב

whoami \\ משתמש להבנת המשתמש הנוכחי נוח במיוחד במצב SSH
history - \\ לחפש סיסמאות ביוזרים שלא מחקו היסטוריה
clear - ctrl l
passwd - שינוי סיסמה לא להשתמש ב
root toor
passwd -d \\ יצירת משתמש ללא סיסמה

wc - ספירת מילים

cat /etc/passwd
cut -d ":" -f 1,2,3 /etc/passwd
d: <delimiter>

crunch 1 5 1234567890 -o pass.lst \\ מכין קובץ לפריצה

sort hi.txt
sort -r hi.txt <reverse>
cat 12345123345 > file.txt
sort file.txt | uniq

## tail / head shows 10 lines by default

head -n 2 file.txt
tail -f file.txt \\ משאיר את הקובץ פתוח ורואים תוספות של שורות בזמן אמת

touch "john mogi"
rm john/ mogi

cut -d ":" -f 1 group
cut -d : -f 1 group
