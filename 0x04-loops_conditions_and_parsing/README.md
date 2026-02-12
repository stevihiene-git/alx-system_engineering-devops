loops and condition parsing
Task 6 can also be written as follows:

i=1;

while [ $i -le 20 ]
do
    case $i in 
        4)  echo "bad luck from China";;
        9)  echo "bad luck from Japan";;
        17) echo "bad luck from Italy";;
        *)  echo "$i";;  # This catches everything else
    esac
    ((i++))
done
