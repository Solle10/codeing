# codeingame

# Hacking at Robbercity

import sys
import math



m1 = bytes.fromhex(input())  # M ^ A
m2 = bytes.fromhex(input())  # M ^ A ^ B
m3 = bytes.fromhex(input())  # M ^ B




xorbyte = bytes(m1^m2^m3 for m1,m2,m3 in zip(m1,m2,m3))
print(xorbyte.decode())





# Decode the message
import sys
import math


p = int(input())
c = input()

Write an answer using print
 debug: print("Debug messages...", file=sys.stderr, flush=True)

answer=""

while p>=len(c):
    answer+=c[p%len(c)]
    p=int(p/len(c))-1
print(answer+c[p])
