#!/bin/bash

length=8
level=1

if [ $# -eq 2 ]; then
    if [ "$1" = "-l" ];then
        length=$2
    elif [ "$1" = "-L" ];then
        level=$2
    fi
    if [ $level -eq 1 ]; then
        tr -dc 'A-Za-z' < /dev/urandom | head -c $length
    elif [ $level -eq 2 ]; then
        tr -dc 'A-Za-z0-9' < /dev/urandom | head -c $length
    elif [ $level -eq 3 ]; then
        tr -dc 'A-Za-z0-9@#$%&?><' < /dev/urandom | head -c $length
    else
        echo  "Invalid arguments"
    fi
elif [ $# -eq 4 ]; then
    if [ "$1" = "-l" ]; then
        length=$2
        level=$4
    elif [ "$1" = "-L" ]; then
        length=$4
        level=$2
    fi
    if [ $level -eq 1 ]; then
        tr -dc 'A-Za-z' < /dev/urandom | head -c $length
    elif [ $level -eq 2 ]; then
        tr -dc 'A-Za-z0-9' < /dev/urandom | head -c $length
    elif [ $level -eq 3 ]; then
        tr -dc 'A-Za-z0-9@#$%&?><' < /dev/urandom | head -c $length
    else
        echo  "Invalid arguments"
    fi
else
    echo "use genpasswd -l <length> -L <LEVEL [1-3]>"
fi
