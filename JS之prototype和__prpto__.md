**实例对象的__prpto__等于其构造函数prototype**</br>
**prototype的意思是原型对象**</br>

实例对象中会含有一个隐藏属性__prpto__，里面放的是由它的构造函数构造出来的实例对象们所共有的属性。</br>
调用该实例对象的属性，找不到时就会来这个隐藏属性中找，这个隐藏属性找不到就在隐藏属性的隐藏属性__prpto__中找。</br>

目的是：减少重复，节省空间。</br>
```
let a=[];
a.__prpto__===Array.prototype;//true
a.__prpto__.__prpto__===Object.prototype;//true 
```

因为Array的构造函数是Object。</br>

所以调用a.hasOwnProperty时，a没有；</br>
就去a.__proto__中找（即Array.prototype），发现还是没有；</br>
就去a.__prpto__.__prpto__（即Array.prototype.__prpto__），也就是Object.prototype中找，于是找到了。</br>


**Object.prototype.__proto__的结果是null **
**Array.prototype还是Array**

```Array.isArray(Array.prototype); // true```
