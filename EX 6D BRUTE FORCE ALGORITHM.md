# EX 6D BRUTE FORCE ALGORITHM
## DATE:
## AIM:
To write a python program using brute force method of searching for the given substring in the main string.

## Algorithm
1.Take two inputs: the main string and the substring to search for.

2.Create a regex pattern using the substring.

3.Search for the first match of the pattern in the main string.

4.If a match is found.Print the starting index of the match.

5.Continue searching for the next match, starting just after the current match.

6.Repeat step 4 until no more matches are found.   

## Program:
```
# Developed by: Dharani P
# Register Number: 212222220011

import re
def match(string,sub):
    pattern = re.compile(str2)
    r = pattern.search(str1)
    while r:
        print("Found at index {}".format(r.start()))
        r = pattern.search(str1,r.start()+1)    

str1=input()
str2=input()
```

## Output:
![447235462-4147a9db-7fd1-44cc-8b0c-6173a5d35215](https://github.com/user-attachments/assets/d1803ffb-da92-4728-bc70-aa1ff4c6f113)




## Result:
Thus the above program was executed successfully for searching the substring at respective index.
