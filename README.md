# exercise
x = int(input("Please enter first integer: "))
y = int(input("Please enter second integer: "))
if (x == y):
    print("两数相同！")
elif (x > y):
    print("较大数为：",x)
else:    
    print("较大数为：",y);
,b,c=3,4,5
if a <= b:
    if c < b:
        print ("b是最大的数")
    else:
        print ("c是最大的数")
else:
    if c < a:
        print ("a是最大的数")
    else:
        print ("c是最大的数")
sum=0
for x in range(1,101):
   if x % 2==0:
       print(x)
       sum=sum+x
print("累加和是:",sum)
year = int(input("Please enter the year: "))
if  ((year%4==0 and year%100!=0) or (year%400==0)):
    print(year,"is a leap year.")
else:
    print(year,"is not a leap year.")
cunkuan = 10000  #本金10000元
years=0
while cunkuan<20000:
       years+=1
       cunkuan=cunkuan*(1+0.0325)
print(str(years)+"年以后，存款会翻番")
score=int(input('请输入成绩（0～100）：'))
if score > 100:
    grade = "输入错误！"
elif score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
elif score >= 70:
    grade = 'C
elif score >= 60:
    grade = 'D'
elif score >= 0:
    grade = 'E'
else:
    grade = "输入错误！"
print(grade)
num=7
while True:
    guess=int(input('请输入你猜的数（0～9）：'))
    if guess == num:
        print("恭喜！你猜中了！")
        break;
    elif guess > num:
        print("太大")
    else:
        print("太小")
import math
n=int(input("请输入一个数:"))
x=int(math.sqrt(n))
i,w=2,0
for i in range (2,x+1):
     if n%i==0:
         w=1
if w==1:
    print(n,"不是素数。")
else:
    print(n,"是素数。")
hour,minute,second=input('请输入一个时间（h:m:s）:').split(':')
hour=int(hour)
minute=int(minute)
second=int(second)
second+=30
if second >= 60:
    second = second-60
    minute += 1
minute+=5
if minute >= 60:
    minute = minute-60
    hour += 1
if hour == 24:
    hour = 0
print('%d:%d:%d'%(hour,minute,second))
m=1000
for a in range(2,m+1):
    s=a
    L1=[]
    for i in range(1,a):
        if a%i==0:
            s-=i
            L1.append(i)
    if s==0:
        print("完数：%d，因子包括："%a,end="")
        for j in range(1,len(L1)):
            print("%d"%L1[j],end=",")
        print("\n")
day=9
x=1
while day>0:
    x=(x+1)*2
    day-=1
print("total=",x)
x = int(input("Please enter first integer: "))
y = int(input("Please enter second integer: "))
print("The sum is:");
print(x+y);
for i in range(len(L1)):
    L1[i]=int(L1[i])
    L2[i]=int(L2[i])
maxVal=L1[0]
maxDay=0
minVal=L2[0]
minDay=0
flname="temp.txt"
f=open(flname)
ht=(f.readline()).strip()
L1=list(ht.split(','))
lt=(f.readline()).strip()
L2=list(lt.split(','))
f.close()

for i in range(1,len(L1)):
    if L1[i]>maxVal:
        maxVal=L1[i]
        maxDay=i
    if L2[i]<minVal:
        minVal=L2[i]
        minDay=i
print("这周第"+str(maxDay+1)+"天最热，最高"+str(maxVal)+"摄氏度")
print("这周第"+str(minDay+1)+"天最冷，最低"+str(minVal)+"摄氏度")
