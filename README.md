# Day3_First-positive-integer

''' Given an array of integers,find the first missing positive integer in linear time and constant space.

In other words find the lowest positive integer that does not exist in the array.

The array can contain duplicate and negative numbers



[3,4,1,-1] == 2

[1,2,0]==3 '''



arr=list(map(int,input().strip().split()))

count=0

maxel=max(arr)

for i in range(1,maxel+1):

    if i not in arr:

        print(i)

        count=count+1

    

else:

     if(count!=1):

         print(maxel+1)
