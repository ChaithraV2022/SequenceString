# SequenceString
Number of Times characters in string in sorted order
n=input()
n="".join(sorted(n))
a=dict()
r=''
for i in n:
    if i in a.keys():
        a[i]+=1
    else:
        a[i]=1
for k,v in a.items():
    r+=("%s%d"%(k,v))
print(r)
