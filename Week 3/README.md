# Week3   

* Debug  
  assert \<expression\> , \<string\> -> if not expression, string  
  assert x>0 -> x<=0报错  
* Test  
  \>\> f(1)  
  1  
  \>\> f(2)  
  3  
* Raise Statement  
  raise \<expression\>  
  raise TypeError('you have the wrong type')  -> 运行到raise这步便会报后面的错  
  其他类型的Error : NameError, KeyError, RuntimeError  
* Try Statements  
  try:  
  &nbsp;&nbsp;&nbsp;&nbsp;\<try suite\>  
  except \<exception class\> as \<name\>:  
  &nbsp;&nbsp;&nbsp;&nbsp;\<except suite\>   
    
  try:  
  &nbsp;&nbsp;&nbsp;&nbsp;return f(x)  
  except ZeroDivisionError[as e]:  
  &nbsp;&nbsp;&nbsp;&nbsp; print('handled'[, e])  
  &nbsp;&nbsp;&nbsp;&nbsp; return 0  
* sum函数  
  sum(iterable, start) -> start + []内所有数字  
  sum([[2, 3], [4]], [ ]) -> [2, 3, 4]  
* max函数  
  max(iterable, func) ->对iterable参数都进行func操作，返回使f(x)最大的x值  
  \>\> max(range(10), lambda x: 7 - (x-2) * (x-4))  
  3  
* all函数  
  all([iterable]) ->判断iterable中所有元素是否为True,是则返回True,反之为False  
