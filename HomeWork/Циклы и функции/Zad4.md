#!/bin/bash
why="^[0-9]+$"
nul=0
echo Введите числа:
echo первое число
read num1
echo второе число
read num2
if [[ $num1 =~ $why ]] && [[ $num2 =~ $why ]]; then
    select act in summa raznost proizvedenie delenie; do
    case $act in

summa)
echo сумма $(($num1+$num2)); break;;

raznost)
echo разность $(($num1-$num2)); break;;

proizvedenie)
echo произведение $(($num1*$num2)); break;;

delenie)
if [ $num2 -eq $nul ]; then
    echo "деление на 0!";
    else
        echo целочисленное деление $num1 на $num2
        echo $(($num1/$num2))
        echo остаток от деления $num1 на $num2
        echo $(($num1%$num2))
fi;

esac
done;
else
echo "не число, введите число">&2; exit 1
fi;
fi;
