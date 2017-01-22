# MergeSort
Python program that demonstrates how merge sort works in terms of splitting and merging. Each phase of items in the array getting split and then merging is shown in the program. 

Algorithm:

Merge(L,R,A)
nL <- length(L)
nR <- length(R)
i=j=k=0
while(i<nL && j<nR){
if(L[i]<=R[j]){
A[k] = L[i]
i+=1
}
else{
A[k] = R[i]
j+=1
}
K+=1
}
while(i<nL){
A[k] = L[i]
i+=1
k+=1
 }
while(j<nR){
A[k] = R[j]
j+=1
k+=1
 }
 
 Sort(A)
 n<- length of A
 if(n<2) return
 mid = n/2
 leftarray = array of size from 0 to mid
 rightarray = array of size from mid to n
 for i=0 to mid
 leftarray[i]=A[i]
 for i=mid to n
 rightarray[i] = A[i]
 Sort(leftarray)
 Sort(rightarray)
 Merge(leftarray,rightarray,A)
 

