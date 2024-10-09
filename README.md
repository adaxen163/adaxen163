ls=(3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20)
ind=[0]
rrr=str()
n=int(input('Введите число: '))
for i in range(1, len(ls)):
    for j in range(i + 1, len(ls)):
        if n % (i + j) == 0 and ls != j and i!=0 and j!=0:
            rrr += (str(i) + str(j))
print(rrr)
