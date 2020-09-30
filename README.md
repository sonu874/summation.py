# summation.py

def summation(l,p,s):
    m=[];i=0
    
   while i<len(l):
        m=l[i:p]
        if sum(m==s):
            print(m)
            i=i+1
            p+=1
         else:
            i=i+1
            p=p+1
   

#main
l=[]
n=int(input("enter length of array:"))
for i in range(n):
    x=int(input("enter a value:"))
    l.append(x)
s=int(input("enter a given sum:"))
for p in range(n):
    x=summation(l,p,s)
