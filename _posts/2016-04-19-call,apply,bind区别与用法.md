---
layout: post
title: call,apply,bind区别与用法
categories: js
description: call,apply,bind区别与用法
---
 Arguments 对象
JavaScript 函数有个内置的对象 arguments 对象。
argument 对象包含了函数调用的参数数组。
通过这种方式你可以很方便的找到最大的一个参数的值：
 
 
<pre>
x = findMax(1, 123, 500, 115, 44, 88);
 
function findMax() {
    var i, max = arguments[0];
    
    if(arguments.length < 2) return max;
 
    for (i = 0; i < arguments.length; i++) {
        if (arguments[i] > max) {
            max = arguments[i];
        }
    }
    return max;
}
document.getElementById("demo").innerHTML = x;
 
</pre>
 
 查找最大的数。 
 500
 