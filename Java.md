## 向下转型

short占据16位，int占据32位，float占据32位，double占据64位

不能隐式执行向下转型，这样会使精度降低。

```java
float f = 1.1; //错误
```

```java
float f = 1.1f; //正确
```

```java
short s1 = 1; //错误，short精度低，int精度高，不能直接转换
```

```java
s1 += 1; //正确，隐式类型转换
//相当于
s1 = (short)(s1+1); 
```

