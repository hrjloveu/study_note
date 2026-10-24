

---
### HelloWorld

```c
#include <stdio.h>  
int main() {
	printf("Hello World!");  
	return 0;
}
```

每行有效代码后面都要加 ;

---

### 注释规则

单行注释
```c
//text
```


多行注释
```c
/*text1
text2*/
```


---
### 输出
输出纯文本
```c
printf("Hello World!\n");
```

当我们需要输出变量
```c
int money = 100;
int num = 5;
printf("Money: %d\nNum: %d",money,num);
```
> 输出：  
> Money: 100  
> Num: 5

---
### 输入
`scanf ("格式说明符", &变量名称);`
```c
int num;
scanf("%d", &num); //用户输入整数，并赋值给num
```
被赋值变量前要加`&`


---
