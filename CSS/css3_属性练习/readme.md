# css3 选择器

## 属性选择器

    ~~~
    .class[src="logo.png"]{

    }
    ~~~

    [attribute] 选择带有该属性的所有元素

    [attribute="text1"] text1必须是完整的属性值，就是引号里面所有的东西

    [attribute~="text2"] text2 可以是属性值里，用空格隔开的部分

    [attribute~="text3"] test3 可以是属性值里开头完整结构，或者是“-”前面的单词

css3

    [attribute^="test1"] 属性值以test1开头的

    [attribute$="txt"] 该属性中属性值以txt结尾的元素

    [attribute*="test3"] 属性中包含test3字串的元素

    element:first-of-type 指定的每一组中并列的element属性中的第一个

    element:last-of-type 指定的每一组中并列的element属性中的最后一个

    :first-child 一定要指明父级元素是谁
    :last-child 一定要指明父级元素是谁

    两者的区别：
    first-of-type 相对于并列元素而言
    first-child   相对于父容器而言

    :nth-child    相对于父容器而言
~~~
.father div:nth-child(2n){
}
~~~

## 浮动元素本身不用清除浮动，浮动元素是可以被浮动元素正常撑开的。

## border-radius 

    从左往右顺时针旋转

## box-shadow 

    x-offset y-offset blur spread color

## background-size
    
    contain 只要一条边达到父容器大小，就不再放大

   * cover 永远有一个方向超出，最小一条边达到父容器大小，另外一条边超出

## background-oringin/background-clip

    oringin: 指定，背景图从哪开始
    默认 padding-box 背景图，从padding左上角开始
    content-box 背景图从content左上角开始
    border-box 背景图从border开始

    clip: 
    默认
    content-box
    padding-box
    border-box
    
    background-blend-mode

