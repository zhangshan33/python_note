# python_note
python相关笔记
# !/usr/bin/python
# -*- coding: utf-8 -*-

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
