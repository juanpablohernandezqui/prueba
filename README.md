# prueba
prueba
import numpy as np

def trapecio(a,b,n):
  S=0
  for i in range(n):
    x1 = a + (b-a)*(i)/n
    f1x = (np.log(x1))**(2*x1)
    x2 = a + (b-a)*(i+1)/n
    f2x = (np.log(x2))**(2*x2)
    S+= f1x + f2x
  return S*(b-a)/(2*n)

print(trapecio(1,1.1,10))
print(trapecio(1,1.1,100))
print(trapecio(1,1.1,1000))
print(trapecio(1,1.1,10000))

