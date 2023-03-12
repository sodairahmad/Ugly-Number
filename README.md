# Nth  Ugly-Number. Datastructure


def successive_div(x,y):
    while x % y == 0:
        x = x // y 
    return x 

print(successive_div(6,2))

def Ugly_chec(num):
    num = successive_div(num,2)
    num = successive_div(num , 3)
    num = successive_div(num, 5)
    if num == 1:
        return False
    
print(Ugly_chec(6))

def n_th_ugly(n):
    i = 1 
    counter = 1 
    while n > counter:
        i += 1 
        if Ugly_chec(i):
            counter += 1 
    print(f"The {n}th Ugly number is {i}") 
no = n_th_ugly(15)
print(f"The 15 Ugly number is {no}")
print("sodair ")
    
    
    
