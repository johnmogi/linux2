during grab press e

left shift (hold)
e

exercise:

1 .הריצו 5 פעמים את התוכנה Wireshark מאחורי הקלעים באותו ה-bash.
2 .תהרגו את ה-bash שהריץ את כל ה-Wireshark שהוא בעצם תהליך האבא שלהם, מה קרה לתהליכי ה-
Wireshark האם הם נסגרו?
3 .תהרגו תהליך Wireshark כלשהו מתוך ה-5 תהליכים.
4 .תהרגו את כל 4 תהליכי ה-Wireshark בפקודה אחת.

1. wireshark & ; wireshark & ; wireshark & ; wireshark & ; wireshark & ;  
pidof wireshark
ps -ef | grep wireshark
ps -ef | grep <pid>

kill -15 <pid>
kill -9 <pid>
ps -ef | grep wireshark





