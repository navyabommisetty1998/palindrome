# palindrome
#!/bin/bash
echo "enter the number"
read n
sum=0
temp=$n
  while[ $n gt 0 ]
   do
      r=$(( n % 10 ))
      sum=$(( sum * 10 + r ))
      n=$(( n/10 ))
    done
     if[ $temp -eq $sum ]
     then
       echo "it is a palindrome number"
       else
       echo "it is not a palindrome"
       fi
    
      
