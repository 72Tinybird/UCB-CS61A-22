# Week 1 
Windows系统可在此下载Git：https://git-scm.com/download/win

## ① Lab
* 理解运算符 (Assignment)
## ② Note

* ls : lists all files in the current directory
* cd <path to directory>: change into the specified directory
* mkdir <directory name>: make a new directory with the given name
* mv <source path> <destination path>: move the file at the given source to the given destination
* python -i : run Python code line by line
* python -m doctest : Runs doctests in a particular file
## ③ 作业要点
* Q5 ： 函数套函数每次经过函数会先运行，无return值赋值给其他变量就是None  
  
  \>>>print(print(1), print(2))  
  1  
  2  
  None None
  
* def absolute_value(x)：   # 一个statement(if开始) 三个clause(if,elif,elif) 三个suit(clause下面的内容)  
	if x < 0:  
	&nbsp;&nbsp;&nbsp;&nbsp;return -x  
	elif x == 0:  
  &nbsp;&nbsp;&nbsp;&nbsp;return 0  
	else:  
	&nbsp;&nbsp;&nbsp;&nbsp;return x  

* and和or  
(a and b and c) a真->b真->c(无论真假都输出) 中间有假就输出假(0, False, None)  
(a or b or c)   a假->b假->c(无论真假都输出) 中间有真就输出真

* assert  
def square(r):  
&nbsp;&nbsp;&nbsp;&nbsp;assert r > 0, "r must be positive" #小于等于0时报错  
&nbsp;&nbsp;&nbsp;&nbsp;return r * r
    
* return values  
def make_adder(n):  
	
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;def adder(k):  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return k + n  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return adder  
	
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;make_adder(2000)(19)
