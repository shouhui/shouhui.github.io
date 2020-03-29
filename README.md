# 前端学习

这里记录学习前端总结

** 这里是一段强调语法 **


## 重写前端笔记

这里记录学习总结

* [开篇词](start/README.md)
* [明确前端学习路线和方法](define-pathroad/README.md)
1. 建立知识架构
2. 深入理解重要知识点
* [HTML](html/README.md)
* [CSS](css/README.md)
* [JavaScript](js/README.md)

## 经典面试题
# 基础知识
事件原理,闭包,调用栈,Promise,ES6,工程化,webpack,性能优化,跨域,安全问题,React/Redux思想,Virtual DOM,Diff算法,移动端布局,浏览器渲染原理,Ebent Loop
1. 网页从输入网址到渲染完成经历了哪些过程
2. apply、call、bind函数
3. JavaScript 有几种类型
4. 深浅拷贝
5. 作用域与闭包

作用域定义了变量,函数,对象的可访问范围,有全局作用域/块作用域/函数作用域,内层作用域可以访问外层作用域定义的内容,代码运行时阶段,如果当前作用域找不到变量的引用,就向外层依次查找,直到找到该变量或者到全局作用域都没有找到,这就形成了作用域链. 
词法分析阶段,会函数定义的当前作用域记录到函数的内部对象,作为函数执行时的可访问作用域,也就是说,如果在函数定义的当前作用域同时定义了一个变量,那么执行时函数可访问函数外层作用域的该变量,这样每次调用函数可将该函数外层作用域变量作为共享变量.如果该函数和变量不想让程序其它部分干扰(最小访问原则),那么可以将它们封装在一个新定义的函数内,新函数返回业务需要的内层函数.这样,拥有该内层函数引用的作用域调用函数时候,同时可以访问封装定义在内层函数外的变量,这就形成了闭包
```
var fab = (function() {
    var cache = {};
    function fab (x) {
        if (x < 2) {
            return 1;
        }
        if (!(x in cache)) {
            cache[x] = x * cache[x - 1];
        }
        return cache[x];
    }
    return fab;
})();
var test = fab();
test(8);
```

6. new 操作符具体干了什么
7. js 创建对象的几种方式
8. JS 如何实现一个类
9. Js如何实现继承
10. this 对象的理解
11. 数组去重
12. 宏任务/微任务
13. 盒模型


----

加油吧,少年! 

----
