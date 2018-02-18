# j
print ("WelCoMe iN number scrable ")
x=[1,2,3,4,5,6,7,8,9]
print (x)
p1=[0,0,0,0,0]
p2=[0,0,0,0,0]
c=0
b=0
while True :
    while True :
        z=int(input("player one choose (be careful to choose a number only from the lest)"))
        while (z not in x ):
            z=int(input("player one choose (be careful to choose a number only from the lest)"))
            if (z in x):
                break
        x.remove (z)
        print (x)
        p1[c]=z
        print ("player one choose " ,p1)
        print ("player two choose " , p2)
        c=c+1
        break
    if (x==[]):
        print ("no one wiiin ")
        break
    elif ((p1[0]+p1[1]+p1[2]==15) and (p1[0]*p1[1]*p1[2] !=0)) \
        or ((p1[1]+p1[2]+p1[3]==15) and (p1[1]*p1[2]*p1[3] !=0)) \
        or ((p1[2]+p1[3]+p1[4]==15)and (p1[2]*p1[3]*p1[4] !=0))  \
        or ((p1[0]+p1[3]+p1[4]==15)and (p1[0]*p1[3]*p1[4] !=0)) \
        or ((p1[0]+p1[2]+p1[3]==15)and (p1[0]*p1[2]*p1[3] !=0)) \
        or ((p1[1]+p1[3]+p1[4]==15)and (p1[1]*p1[3]*p1[4] !=0)) \
        or ((p1[0]+p1[1]+p1[3]==15) and (p1[0]*p1[1]*p1[3] !=0)) \
        or ((p1[0]+p1[2]+p1[4]==15) and (p1[0]*p1[2]*p1[4] !=0)) \
        or ((p1[1]+p1[2]+p1[4]==15) and  (p1[1]*p1[2]*p1[4] !=0)) \
              or ((p1[0]+p1[1]+p1[4]==15) and (p1[0]*p1[1]*p1[4] !=0)):
        print ("player one wiiiiiiiin ")
        break
   
    while True :
        f=int(input("player two choose(be careful to choose a number only from the lest)"))
        while (f not in x):
            f=int(input("player two choose(be careful to choose a number only from the lest)"))
            if (f in x):
                break
        x.remove (f)
        print (x)
        p2[b]=f
        b=b+1
        print (p1)
        print (p2)
        break
    if ((p2[0]+p2[1]+p2[2]==15) and (p2[0]*p2[1]*p2[2] !=0))\
        or ((p2[1]+p2[2]+p2[3]==15)and (p2[1]*p2[2]*p2[3]!=0))\
        or ((p2[2]+p2[3]+p2[4]==15)and (p2[2]*p2[3]*p2[4] !=0))\
        or ((p2[0]+p2[3]+p2[4]==15)and (p2[0]*p2[3]*p2[4] !=0))\
        or ((p2[0]+p2[2]+p2[3]==15)and (p2[0]*p2[2]*p2[3] !=0))\
        or ((p2[1]+p2[3]+p2[4]==15)and (p2[1]*p2[3]*p2[4] !=0))\
        or ((p2[0]+p2[1]+p2[3]==15)and (p2[0]*p2[1]*p2[3] !=0))\
        or ((p2[0]+p2[2]+p2[4]==15)and (p2[0]*p2[2]*p2[4]!=0))\
        or ((p2[1]+p2[2]+p2[4]==15)and (p2[1]*p2[2]*p2[4]!=0))\
        or ((p2[0]+p2[1]+p2[4]==15) and (p2[0]*p2[1]*p2[4]!=0)):
        print ("player two wiiiiiin")
        break
