# 记录一些题目

## JavaScript和ECMAScript概念上有什么区别？
```text
答：JavaScript包含ECMScript
```

## 如何在HTML中引入JavaScript？
```text
答：使用<script>标签嵌入
```

## Chrome, Firefox, IE分别如何关闭JavaScript功能？
```text
答：
```

## 下面哪些变量名是有效的？
```text
one, oneTwo, 1Two, one$, $One, $1, _One, _1, 1_, one;, one), var, true, null, undefined
```
```text
答：one,onetwo,one$,$One,$1，_One, _1
```

## JavaScript的数据类型有哪几种？
```text
答：undefined,null,string,number,boolean,object
```

## 不运行代码，写出下面代码的结果
```javascript
1. console.log(null == undefined);
2. console.log(null === undefined);
3. console.log(null == abc); // abc is not defined
4. console.log(typeof null == typeof undefined);
5. console.log(typeof(null) == typeof(undefined));
6. console.log(typeof 'string' == typeof 'undefined');
7. console.log(typeof {} == typeof []);
8. console.log(typeof null == typeof []);
9. console.log(1 == true);
10. console.log(0 === false);
11. console.log(true === Boolean('a'));
12. console.log(typeof 1 == typeof true);
13. console.log(typeof 1 == typeof 0.1);
14. console.log(0.1 + 0.2 == 0.3);
15. console.log(9007199254740992 + 1);
16. console.log(070 == 70);
17. console.log(08 == 8);
18. console.log(10.0 === 10);
19. console.log(isNaN(NaN));
20. console.log(NaN == NaN);
21. console.log(Number(''));
22. console.log(parseInt(''));
23. console.log(parseInt('.01'));
24. console.log(parseFloat('.01'));
```

```text
答：
    1.true
    2.false
    3.Undefined
    4.false
    5.false
    6.true
    7.true
    8.true
    9.true
    10.false
    11.false
    12.false
    13.true
    14.true  //false
    15.9007199254740992
    16.true  //false
    17.true
    18.false  //true
    19.true
    20.true  //false
    21.NaN   //0
    22.NaN
    23.NaN
    24.0.01



```

## 字符串使用单引号和使用双引号表示有什么区别？比如'abc', "abc"
```text
答：没有区别，但使用双引号开始就要以双引号结束，单引号也是如此

## 列举常用的字符串方法，比如String.length()
```text
答：toString()
```

## 方法String.substr()和String.substring()有什么区别？
```text
答：
```

## 下面代码输出是什么？
```javascript
var lang = 'JavaScript';
var myLang = lang;
lang = 'Java';
console.log(mylang);
```
```text
答：JavaScript
```

## 下面代码输出是什么？
```javascript
var number = 11;
console.log(11 == number.toString());
console.log(11 === number.toString());
console.log(String(11) === number.toString());
console.log(11 + '' === number.toString());
```
```text
答：
true
false
true
true

```

## 写出你对JavaScript“对象”概念的理解？
```text
答：
```

## 什么是一元操作符？分别有哪些？
```text
答：只能操作一个值的操作符
   递增和递减操作符
   一元加和减操作符
```

## 下面代码输出是什么？
```javascript
var age = 23;
++age;
age--;
age = age + 1;
console.log(age++);
console.log(++age);
```
```text
答：24
   26
```

## 下面代码输出是什么？
```javascript
var ageStr = '23';
console.log(ageStr++);
console.log(++ageStr);
```
```text
答：23
   25
```

## 下面代码输出是什么？
```javascript
var ageStr = '23';
console.log(ageStr+);
console.log(+ageStr);
```
```text
答：
   23
```

## 下面代码输出是什么？
```javascript
var isAge = true;
console.log(isAge++);
console.log(++isAge);
``` 
```text
答：1
    3
```

## 下面代码输出是什么？
```javascript
var isAge = true;
console.log(-isAge);
console.log(-isAge);
``` 
```text
答：-1
   -1
```

## 下面代码输出是什么？
```javascript
var isAge = false;
console.log(isAge++);
console.log(++isAge);
```  
```text
答：0
   2
```

## 下面代码输出是什么？
```javascript
var isAge = false;
console.log(+isAge);
console.log(++isAge);
```  
```text
答：0
   1
```

## 下面代码输出是什么？
```javascript
console.log(!false);
console.log(!"blue");
console.log(!0);
console.log(!NaN);
console.log(!"");
console.log(!12345);
console.log(true && false);
console.log(true && false && true);
console.log(true || false);
console.log(true || false || false);
console.log(5 > 3 || 2 < 3 || 1 > 0);
```  
```text
答：
    1.true
    2.false
    3.false
    4.true
    5.true
    6.false
    7.false
    8.false
    9.true
    10.true
    11.true
```

## 下面代码输出是什么？
```javascript
console.log(5 + '5');
console.log(5 + +'5');
```  
```text
答：55
   10
```

## 下面代码输出是什么？
```javascript
console.log(true ? 1 : 0);
console.log(5 > 5 ? 1 + 1 : 1 + 2);
```  
```text
答：1
   3
```

## 下面代码输出是什么？
```javascript
function adjustNumber(i) {
    if (i > 25) {
        console.log("我大于25.");
    } else if (i < 0) {
        console.log("我小于0.");
    } else {
        console.log("我在0到25之间.");
    }
}
adjustNumber(0);
```  
```text
答：我在0到25之间.
```

## 下面代码输出是什么？
```javascript
var i = 0;
do {
    i += 2;
} while (i < 0);
console.log(i);   
```  
```text
答：2
```

## 下面代码输出是什么？
```javascript
var i = 0;
while (i < 0) {
    i += 2;
}
console.log(i);   
```  
```text
答：0
```

## 下面代码输出是什么？
```javascript
var count = 10;
for (var i = 0; i < count; i += 2) {
    console.log(i);
}
```  
```text
答：
    0
    2
    4
    6
    8
```

## 用while改写下面代码？
```javascript
var count = 10;
for (var i = 0; i < count; i += 2) {
    console.log(i);
}
```  
```text
答：
    var count = 10;
    var i = 0;
    while(i<count){
       console.log(i);
       i += 2;
   }
```

## 下面代码输出是什么？
```javascript
var num = 0;
for (var i = 1; i < 10; i++) {
    if (i % 3 == 0) {
        break;
    }
num++;
}
console.log(num);
```  
```text
答：
```2

## 下面代码输出是什么？
```javascript
var num = 0;
for (var i = 1; i < 10; i++) {
    if (i % 3 == 0) {
        continue;
    }
num++;
}
console.log(num);
```  
```text
答：6
```

## 下面代码输出是什么？
```javascript
var i = 35;
switch (i) {
case 25:
    console.log("25");
case 35:
    console.log("35");
case 45:
    console.log("45");
default:
    console.log("Other");
}
```  
```text
答：35
```

## 下面代码输出是什么？
```javascript
function sayHi(name) {
    console.log('Hi ' + name);
    return;
    console.log('Hi ' + name + ' again');
}

sayHi('Lynn');
```
```text
答：Hi Lynn
```

## 下面代码输出是什么？
```javascript
function sayHi(name) {
    console.log('Hi ' + name);
}

function sayHi(name) {
    console.log('Hello ' + name);
}

sayHi();
```
```text
答：Hello Undefined
```

