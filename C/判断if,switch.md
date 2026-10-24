
---

### if判断

```c
int Num = 10; // 这是一个正数还是负数？  
  
if (Num > 0) {  
  printf("该值为正数。");  
} else if (Num < 0) {  
  printf("该值为负数。");  
} else {  
  printf("该值为0。");  
}
```

---

### if简写

`(判断条件) ? 如果为真执行的代码 : 如果为假执行的代码`

例如

```c
int grade = 61;
(grade >= 60) ? printf("pass") : printf("fall");
```

---
### switch case（简易的if）
```c
int num = 5;
switch (num) {
	case 1:
		print("1")
		break;//跳出 `switch` 块并停止执行
	case 2:
		print("2")
	    break;
	default://在没有case匹配时要运行的代码
		print("3")
}
```

如果需要跳出case判断，需要`break`

---