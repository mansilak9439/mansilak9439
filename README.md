- š Hi, Iām @mansilak9439
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
mansilak9439/mansilak9439 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import re

#Extracting Digits and Summing them
hand = open("Week 1 Sample Text.txt")
numlist = []

for line in hand:
    line = line.rstrip()
    extract = re.findall("([0-9]+)", line)

    if len(extract) < 1 : continue

    for i in range(len(extract)):
        num = float(extract[i])
        numlist.append(num)

print(sum(numlist))
