practice
========

bsearch#2 

def binarySearch(BCL , Points):
    low = 0 
    high = len(BCL) - 1
    while low <= high:
        middle = (low+high)/2
        if BCL[middle] < Points:
             low =middle + 1
        if BCL[middle]== Points:
             middle= middle/2
        elif Points <BCL[middle]:
            high = middle - 1
            return middle
        else:
            return -1
       
