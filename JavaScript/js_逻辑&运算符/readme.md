# 1 javascript 基础复习
 
 ## 变量类型

 ## tpyeof parseInt parseFloat 

 ## 数学运算符
    
    + - * / %


# 2 运算符

## 2.0  分类

*   数学运算符(Arithmetic operators)	
*	比较运算符(Comparison operators)
*	逻辑运算符(Logical operators)
*	赋值运算符(Assignment operators)
*	按位运算符(Bitwise operators)
*	条件 (三元) 运算符(Conditional operator)

## 2.1 数学运算符

*   不纯的字符串和undefined是不能帮你进行隐式转换的，结果都是NaN。

*   然后字符串"4ab"、false、true、null都能进行隐式转换。

*   加号比较特殊，面对字符串"4ab"没有隐式转换的。

## 2.2 关系运算符

*   >	大于
*   <	小于
*   >= 	大于等于
*   <=	小于等于
*   ==	等于    
~~~
    var a = 3;
    var b ="3";
    console.log(a == b);    //  true
    console.log(a === b);   //  false
    console.log(a != b);    //  false
    console.log(a !== b);   //  true
~~~

*   !=	不等于
*   ===	全等于
*   !==	不全等


### 字符串和编码

*   string 和 string 也能够进行关系运算，比较的就是字符编码顺序。
~~~
    1	"a" < "b" //true
    2	"A" < "B" //true
    3	"A" < "a" // true ，大写字母在字符集里面是在小写字母前面。
    4	"1" < "A"  //true ，数字在字母前端
    5	"blank" < "blue"  //true   因为一位一位比，直到比出大小。
    6	"25678" < "3"   //true  因为是string和string比，比的是字符编码顺序。
~~~

*   与数字进行关系运算时，纯数字字符串被转为数字，null转换为0，true转换转为1， false转换为0。

*   NaN不等于自己，不全等于自己。
~~~
    1	NaN == NaN  //false
    2	NaN === NaN  //false
    3	NaN != NaN //true
    4	NaN !== NaN //true
~~~

*   string 和 number比，string会被隐式转换为number。
~~~
    1	"25" < 3  //false
~~~

## 2.3 逻辑运算符

*   三个：
    && 	逻辑与运算
    ||	逻辑或运算
    !	逻辑非运算
    正统来说，参与逻辑运算的是boolean和boolean，得到的结果也是boolean值按照真值表来定

    负性的：false，null， 0， NaN， 空字符串("")，undefined
    正性的：除了上面的，全是正性的。
    也就是说，本质上计算机进行a&&b运算的时候，如果a是负性的，那么直接扔出a；如果a是正性的，直接扔出b。

## 2.4 赋值运算符

    =	赋值
    +=	简便写法
    -=	简便写法
    *=	简便写法
    /=	简便写法
    %=	简便写法
    ++
    --
    
    ++可以与输出语句写在一起，++写在变量前和写在变量后不是一个意思。
        a++ : 先用a的原值，然后a加1；
        ++a ：先给a加1，然后用a的新值

# 3 条件分支语句

## 3.1 if语句？

*   如果……否则……  ， 让程序出现分支。
~~~
    可以没有else部分

    如果要执行的语句，只有一行语句，那么就是单行if，就可以省略大括号。
    注意if语句是一个结构体，注意哪些语句是在结构体中，哪些语句不是结构体。
~~~

*   多分支的if

## 3.2 switch case 语句

    简化了if……else……的书写

## 3.3 三元运算符

    ? :是一组运算符，这是JS中唯一一个需要三个元素参加的运算符。
    条件?语句1:语句2


### 浮点数 丢失精确度