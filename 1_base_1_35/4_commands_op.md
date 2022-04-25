& העבר לרקע - למשל  wireshark
fg 1 - העבר קדימה
bg 1 - העבר אחורה

&&  התניה בצע רק אם הפעולה הקודמת הצליחה
ls Downloads && touch ok
|| התניה בצע רק אם הפקודה הקודמת לא הצליחה
ls notFound || touch works

ifconfig > file.txt
שרשור פעולות ו
Stdin
ifconfig < ok > file.txt

ifconfig | grep 0.0
תריץ פילטר על רפטי הרשת וסמן לפי מספר
grep 'hi'
חיפוש בקבצים אחר סטרינג



grep -rni 'frame' * // חיפוש רקורסיבי

חיפוש אחר המילה פריים, תציג לי באופן רקורסיבי עם קייססנסטיב את מיקום המילה בקובץ...

ls > log \\ זרקתי stdin לקובץ
ls > tee log \\ גם שלחתי לקובץ וגם למסך

> file.txt \\ קיצור דרך לטאץ'
