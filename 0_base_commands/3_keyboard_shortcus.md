ctrl l - clear
ctrl pgup pgdwn

ctrl a - start of line
ctrl e - end of line
ctrl u - del line

ctrl c - exit
ctrl z- move program to bg

0 stdin - קלט
1 stdout - פלט
2 stderr - שגיאה

> כתוב לתוך קובץ
> instead of touch

> > הוסף לתוך קובץ

< שליחת פלט + דריסת תוכן הקובץ
<< שליחת פלט תוך כדי שמירה על התוכן הקיים ( append)
& להריץ את התוכנה ב-background, נושא שנלמד בLPI 101-.
wireshark &

&& אם הפעולה הקודמת בוצע בהצלחה בצע גם את הפעולה הנוספת.
|| בצע פקודה שנייה רק אם פקודה ראשונה לא הצליחה
; הרצת פקודה נוספת בין אם הפעולה הראשונה הצליחה ובין אם לא.
< קבלת קלט מקובץ מה שנראה כך wc < roman.txt
| מעבר של stdout ל-stdin של פקודה נוספת.

חיפוש בכל הקבצים במקום הנוכחי
grep "roman" \*

חיפוש רקורסיבי בתת קבצים
grep –rni "roman" \*
tee - פקודה ששולחת את ה-stdout גם לקובץ וגם למסך
ls | tee roman.txt
לא כל פקודה מקבלת stdin באמצעות "|" לכן ישנו משתנה עזר שמוסיף stdin לפקודה הנקרא xargs:
ls | xargs echo
ההבדל בין  
wc file.txt
wc 0< file.txt
הוא שבפלט השני הפקודה לא יודעת מה שם הקובץ שאיתו היא עובדת
יצירת קובץ ריק

> file.txt
