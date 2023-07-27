# Python-13-
Python学习笔记(13)
# p44 嵌套循环
‘’‘输出三行四列的矩形’‘’
for i in range(1,4): #行表，执行三次，一次一行
    for j in range(1,5):
        print('*',end='\t') #不换行输出
    print()

for i in range(1,10): #行数
    for j in range(1,i+1):
        print(i,'*',j,'=',i*j,end='\t')
    print()



# p45 二重循环的break与continue
for i in range(5):  #代表外层循环要循环5次
    for j in range(1,11):
        if j%2==0:
            #break
            continue
        print(j,end='\t')
    print()
#跳过内层循环，不影响外层循环



# p46 为什么需要列表
#列表可以存储多个不同的数据类型
a=10  #变量存储的是一个对象的引用
lst=['hello','world',98]
print(id(lst))
print(type(lst))
print(lst)
#列表存储的id的存储对象是三个元素的id
