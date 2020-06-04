
maven：
https://maven.apache.org/plugins/maven-shade-plugin/examples/class-relocation.html


# volatile

volatile修饰的变量如果是对象或数组之类的，其含义是对象获数组的地址具有可见性，但是数组或对象内部的成员改变不具备可见性

# final

java内存模型对final域遵守如下两个重拍序规则

+ 初次读一个包含final域的对象的引用和随后初次写这个final域，不能重拍序。
+ 在构造函数内对final域写入，随后将构造函数的引用赋值给一个引用变量，操作不能重排序。

以上两个规则就限制了final域的初始化必须在构造函数内，不能重拍序到构造函数之外，普通变量可以。

# this引用逃逸

```
https://blog.csdn.net/u010571316/article/details/77993309
```

