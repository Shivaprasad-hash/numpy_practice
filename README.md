# numpy_practice
#Creating Arrays from numpy with functions

# f1 array()

# #1D array
import numpy as np
a = [1,2,3,4]
b= np.array(a)
print(b)
print()

# 2D array
c = [[1,2],[3,4]]
d=np.array(c)
print(d)
c[0][0]
print()

# 3D array
e = [[5,6],[7,8],[9,10]]
f = np.array(e)
print(f)
print()
print()

# f2 asarray with nditer
g = [[10,2],[34,23],[12,45]]
h = np.asarray(g,dtype=int,order="C")
for i in np.nditer(h):
    print(i)
print()
j = [[10,2],[34,23],[12,45]]
k = np.asarray(j,dtype=int,order="F")
for i in np.nditer(k):
    print(i)
print()

# f3 frombuffer
l = b"Shiva prasad"
m = np.frombuffer(l,dtype="S1")
print(m)
print()

# f4 fromiter
n = [1,2,3,4]
o = np.fromiter(n,dtype=int,count=2)
print(o)
print()
