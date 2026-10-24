


---

结构体可理解为数据库


### 创建结构体
```c
struct date { //声明结构体  
	int year;  
	int month;  
	int day; //结构体中的成员  
};  

struct date today; //创建结构体变量  

today.year = 2001;  
today.month = 9;  
today.day = 11; //为成员赋值  

printf("%d-%d-%d\n", today.year, today.month, today.day); //调用结构体
```

也可以用以下方式给成员赋值

```c
struct date today = {2001, 9, 11};
```

或是

```c
struct date today = {.year = 2001, .month = 9, .day = 11};
```

当需要改变成员的值，也可以使用以下方法
```c
today = (struct date) {2001, 9, 11};
```

并且，结构体变量还能做到数组做不到的赋值方法

```c
today = yesterday;
```

---

### 结构指针

结构体变量与数组不同，它并不是一个指针，所以必须新建一个指针指向结构体变量，且需要加`&`符号取地址

```c
struct date *p = &today;
```

所以，结构体变量与数组不同，传入函数的是形参

==如果需要用函数更改结构变量的值，可以使用指针，也可以定义一个返回值数据类型为结构体函数==

---