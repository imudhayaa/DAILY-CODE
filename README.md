- 
Given a list of number k , return whether any two numbers from the list add up to k

i.e  given input - [10, 15, 3, 7] and k of 17, return since [10+7] is 17


SOLUTION

a=list(map(int,input().split()))
k=int(input())
for i in a:
    for j in a:
        if(i+j==k):
            print("True")
    break

a=list(map(int,input().split()))
k=int(input())
n=len(a)
b=0
for i in range(n):
    for j in range(n):
        if a[i]==a[j]:
            continue
        if int(a[i]) + int(a[j])==k:
            b=b+1
            if b==1:
                print("True")

