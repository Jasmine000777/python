# python
write sth about python at GitHub
"""
用户身份验证
"""
username=input('请输入口令:\n')
password=input('请输入密码:\n')
if username=='admin' and password=='123456':
    print('身份验证成功!')
else:
    print('身份验证失败!')
    
    
"""
分段函数求值
"""


#拿到题目的做法
x=float(input('请输入x的值:'))
if x>1:
    y=(3*x)-5
    print('f(x)的值为%.1f'%(y))
else:
    if x>=-1:
       y=x+2
        print('f(x)的值为%.1f'%(y))
    else:
        y=(5*x)+3
        print('f(x)的值为%.1f'%(y))
        
#给出的做法1
#对比自己的来看他运用了if--elif--else的结构
#以及他将print作为一次的输出
x = float(input('x = '))
if x > 1:
    y = 3 * x - 5
elif x >= -1:
    y = x + 2
else:
    y = 5 * x + 3
print('f(%.2f) = %.2f' % (x, y))  

#给出的做法二
x = float(input('x = '))
if x > 1:
    y = 3 * x - 5
else:
    if x >= -1:
        y = x + 2
    else:
        y = 5 * x + 3
print('f(%.2f) = %.2f' % (x, y))

"""
英寸和厘米的转换
"""
value=float(input('请输入长度:'))
unit=(input('请输入单位:'))
if unit=='英寸' or unit=='in':
    print('(%.2f)in=(%.2f)cm'%(value,value*2.54))
elif unit=='厘米'or unit=='cm':
    print('(%.2f)cm=(%.2f)in'%(value,value/2.54))
else:
    print('请输入有效字符')
    
    
"""
成绩对应等级
"""
score=float(input('请输入您的成绩:'))
if score>=90:
    grade='A'
elif score>=80:
    grade='B'
elif score>=70:
    grade='C'
elif score>=60:
    grade='D'
else:
    grade='E'
print('您的等级是:',(grade))

"""
判断三条边是否能构成三角形以及计算三角形的周长和面积
"""
a=float(input('请输入边a的值:'))
b=float(input('请输入边b的值:'))
c=float(input('请输入边c的值:'))
if a+b>c and a+c>b and b+c>a:
    l=a+b+c
    p=l/2
    s= (p * (p - a) * (p - b) * (p - c)) ** 0.5
    print('三角形的周长为:',l)
    print('三角形的面积是:',s)
else:
    print('您输入的三条边不能构成三角形')
    
    
