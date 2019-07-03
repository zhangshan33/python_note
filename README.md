# python_note
python相关笔记

#变量赋值
age1 = 18
age2 = age1
age1 = 12
age3 = age2
print(age1,age2,age3)

#整形加法
num1 = 2
num2 = 3
print(num1 + num2)

#字符串加法
s1 = 'a'
s2 = 'bc'
print(s1 + s2)

#字符串乘法
name = '坚强'
print(name*8)

#将用户输入的内容赋值给name变量
name = input("请输入用户名:")
print(name)

#判断条件if
age = input("请输入年龄：")
if int(age) >= 18:
    print("成年了，能干成年人的事情了")

#判断条件 if else
age = input("请输入年龄")
if int(age) >18:
    print("你可以去网吧嗨皮了")
else:
    print("你现在还不行呦")

#多个选项进行单选或者不选 if elif
num = input('请输入要比较的数字：')
if int(num) >=22:
    print('可以工作了')
elif int(num) >=18:
    print("成年了")
elif int(num) <18:
    print("还是小孩子")

#多个选项进行单选（必选） if elif else
num = input("请输入要比较的数字：")
if num > 60:
    print("大了")
elif num < 60:
    print("小了")
else:
    print("猜对了")

#嵌套if
name = input("请输入名字：")
if name == 'meet':
    age = input("请输入年龄：")
    if int(age) == 18:
        print('输入全部正确')
    else:
        print("年龄输入错误！")
else:
    print("名字输入错误")


#while 循环
#为真一直执行，会变成死循环
while True:
    print('I love python')
#有判断条件
flage = True
str_num = input("请输入要比较的数字")
print("进入循环")
while flage:
    if "3" > str_num :
        print("在执行循环")
    else:
        print("要终止循环")
        flage = False
print("退出循环")


#使用while计数
count = 0
while True:
    count = count +1
    print(count)
#控制while循环的次数
count = 0
while count < 100:
    count = count+1
    print(count)

#break 让循环终止
num = 1
while num < 6:
    print(num)
    num += 1
    break
    print("end")


#coutinue 退出当前循环，继续下一次循环
num = 1
while num <6:
    print(num)
    num+=1
    continue
    print("end")

#while else 使用
# 循环一
while True:
    if 3 > 2:
        print('你好')
        break
else:
    print('不好')

# 循环二
while True:
    if 3 > 2:
        print('你好')
print('不好')

#字符串类型
name = input('请输入姓名:')
age = input('请输入年龄:')
job = input('请输入职业:')
hobby = input('请输入爱好:')
msg = '''
------------ info of Alex Li ----------
Name  : %s
Age   : %s 
job   : %s 
Hobbie: %s 
------------- end ----------------

'''
print(msg%(name,age,job,hobby))


#数字类型
name = input('>>>')
s1 = '1234%d'%int(name)
s2 = '1234%i'%int(name)
print(s1)
print(s2)

#转义
num = input('>>>')
s= '目前学习进度:%s%%'%num
print(s)
