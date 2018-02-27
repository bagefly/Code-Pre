# 1 循环语句

## 1.1 for 循环语句

~~~
    for(var i = 1 ; i <= 99 ; i++){
    console.log("第" + i + "次说我爱你");
    }
~~~

## 1.2 穷举思想

# 2 深入学习循环语句

# 2.1 for循环里面的break;和continue;语句

*   break语句
    for循环中，如果遇见了break语句，这个for循环就会立即终止，不在进行其他的迭代了。
    如果你这个break就是想终止所有的循环，那么JS中允许你给循环语句加label。

*   continue语句
    遇见continue语句，for会立即终止执行后面的语句，然后进入下一次迭代了。
    同样的，continue只能中断当前最内层的for，外层for要加label。
    break和continue的目的，就是优化算法的。

# 2.2 do while 语句

语法：
~~~
do{
①语句
}while(②条件表达式)
程序一开始就会执行一次①，然后验证②是否为真，如果是真，继续执行①……
~~~

# 2.3 while语句

while语句是前置验证语句。其余和do while执行效果一样。

