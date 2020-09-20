## 诞生
1995年，布兰登进入网景公司，用10天时间设计出Javascript。当时的Javascript语言实际上是两种语言风格的混合产物----（简化的）函数式编程+（简化的）面向对象编程。提升了上网速度。</br>
因为在这之前，在网页上提交表单，验证结果需要由服务器进行返回，比如必填项没有填...而当时网络速度很慢，等服务器返回结果需要一段时间。而JS直接用浏览器脚本的形式进行校验，提高了提交表单的速度。</br>
网景公司要求蹭一波Java的热度，于是这个语言的命名从Mochac >> LiveScript  >>  JavaScript .实际两个语言并没有实际关系。

## 竞争
JavaScript推出后在浏览器上大获成功，微软公司在1996年8月就为Internet Explorer 3浏览器推出了JScript，以与处于市场领导地位的网景产品同台竞争。</br>
1996年11月，网景向ECMA提交语言标准，由于版权，命名为ECMAScript。</br>
随后，微软将IE浏览器捆绑进Windows，占据市场。</br>
网景内忧外患，将浏览器（Firefox）开源，然而也没有挽救市场，最终被收购。</br>
2001年，IE6随着WindowsXP上市后占据霸主地位（及时没遵循W3C标准，且有安全漏洞）。</br>
2004年，Firefox重生，但只占据一点点份额。</br>
2008年，**Chrome**发布，逐渐扩大市场份额，并在2016年超过IE。</br>

##ECMAScript
1997.11月，第一版。</br>
1999年12月，第三版，使用最广。</br>
第四版，因为功能太多，最终难以实现而流产。</br>
2009年12月，第五版，增加了一些功能。</br>
2015年6月，第六版。</br>
随后，每年发布一版并以年份来命名。</br>

## 10天就写出来的JavaScript的一些奇怪设计
### 类型的隐藏转换
+号作为运算符，有两个含义，可以表示数字与数字的和，也可以表示字符与字符的连接。如果一个操作项是字符，另一个操作项是数字，则数字自动转化为字符。
### null与undefined
**null属于对象（object）的一种，意思是该对象为空，即该处不应该有值**；用处：</br>（1） 作为函数的参数，表示该函数的参数不是对象。（2） 作为对象原型链的终点。</br>
undefined则是一种数据类型，表示未定义。用处：（1）变量被声明了，但没有赋值时，就等于undefined。（2) 调用函数时，应该提供的参数没有提供，该参数等于undefined。（3）对象没有赋值的属性，该属性的值为undefined。
（4）函数没有返回值时，默认返回undefined。</br>
undefined和null在if语句中，都会被自动转为false。</br>
```　var foo;
　　alert(foo == null); // true
　　alert(foo == undefined); // true
　　alert(foo === null); // false
　　alert(foo === undefined); // true
    Number(null);//0
    Number(undefined);//false
    null===undefined;//false
    null==undefined;//true
  ```
  ### NaN
  NaN是一种数字，表示超出了解释器的极限。它有一些很奇怪的特性：
  ``` NaN === NaN; //false
　　NaN !== NaN; //true
　　alert( 1 + NaN ); // NaN ```

## 各语言热度
从百度指数来看，Python近两年是很火了，应该是大数据分析、人工智能带来的热度。JAVA是一门一直以来都很受关注的语言。</br>
JavaScript近几年热度有有较大比例上升，虽然对比其他语言还不是一个水平。</br>
![近10年的前后端百度指数对比](http://chuantu.xyz/t6/741/1600570445x1700468761.png "百度指数对比")
![近10年的JS百度指数变化](http://chuantu.xyz/t6/741/1600570582x2073530529.png "JS百度指数")

参考：</br>
http://www.ruanyifeng.com/blog/2011/06/10_design_defects_in_javascript.html</br>
http://www.ruanyifeng.com/blog/2011/06/birth_of_javascript.html</br>
https://www.ruanyifeng.com/blog/2014/03/undefined-vs-null.html</br>
https://zh.wikipedia.org/wiki/JavaScript#%E5%8E%86%E5%8F%B2</br>


