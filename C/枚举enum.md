
---

枚举是一种用户自定义的数据类型，它代表了一组不可改变的常量

`enum 枚举类型名字{名字0,....,名字n,};`

```c
#include <stdio.h>  
enum COLOR {  //声明枚举
    RED = 5,  //枚举名称
    BLUE = 6,  
    GREEN = 7,  
    NumColors = 3,  
};  
  
int main(void) {  
    enum COLOR c = BLUE;  //定义枚举变量c
    printf("%d", c);  //输出6
    return 0;  
}
```

如果不给枚举名称赋值，则默认为其索引值


---