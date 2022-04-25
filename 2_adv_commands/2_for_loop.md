#!/bin/bash

for i in $(ls) ; do
    echo $i
done

for i in $(find / -name passwd) ; do
    echo $i
done

for i in `ls` ; do echo $i ; done

for i in $( find / -name passwd ) ; do
    echo $i
done

for i in `find / -name passwd` ; do echo $i ; done

for count in `seq 1 10` ; do echo $count ; done


// chmod +x .script.sh

ifconfig | grep "broadcast" | cut -d "t" -f 2 | cut -d " " -f 2

function myIp { ifconfig | grep "broadcast" | cut -d "t" -f 2 | cut -d " " -f 2 ;}
myIp

touch script.sh
!#/bin/bash
function john {
    echo $1 $2
}