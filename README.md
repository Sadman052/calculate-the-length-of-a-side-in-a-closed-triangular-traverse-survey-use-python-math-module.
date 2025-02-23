# calculate-the-length-of-a-side-in-a-closed-triangular-traverse-survey-use-python-math-module.

#program to calculate the length of a side in a 
#closed triangular traverse suirvey whose interior angle is 60.
#The measured length of one side 20 m and corresponding interior angle 30 ,
#use python math module. (hints: a/Sin A = b/Sin B, law of Sines)

import math

def calculation(A, b, B):
    a = b* (math.sin(A)*(math.pi/180))/(math.sin(B)*(math.pi/180))
    return a 

output = calculation(A = 60, b = 20, B = 30)
output = round(output,2)
print("The measured length of the side in meter = ", output)
