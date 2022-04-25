if --> fi
operators:
-lt -> <
-gt -> >
-eq -> ==
-ne -> !=
-le -> <=
-ge -> =>

{script syntax }
variable decleration:
NUM1=100
#echo $NUM1
echo "give me a number:"
read NUM2
if [ $NUM1 -ne $NUM2 ] ; then
    echo "numbers are equal"
elif [ $NUM1 -gt $NUM2 ] ; then
    echo "num1 bigger then num 2"
elif [ $NUM1 -gt $NUM2 ] ; then
    echo "number1 is greater the num2"
else
    echo "numbers are not equal"

fi
