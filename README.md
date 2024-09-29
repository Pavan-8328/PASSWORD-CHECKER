# PASSWORD-CHECKER
p = input()
c = len(p)
spc ='!','@','#','$','%','&','*'
print('Password:- ',p,'\n')

dc =0
for i in p:
 if i.isdigit():
  dc +=1

spcc = 0
for i in spc:
 for j in p:
  if j==i:
   spcc +=1

if c>=7 and dc >=2 and spcc >=2:
  print('Strong')
else:
  print('Weak')
