

---


`typedef 原类型 新名字;`

typedef实际上就是给一个数据类型起一个新名字，改善代码的可读性

```c
typedef int len; //给int类型添加了别名len
len num = 1; //定义了一个类型仍为int的变量num
```

我们也可以使用typedef简化struct复杂的前缀，例如

```c
#include <stdio.h>
int main(int argc, char *argv[])
{
    typedef struct _Student_
    {
        char name[50];
        int age;
        int score;

    } student;

    student stu1 = {"hrj", 18, 99};

    printf("name: %s\n", stu1.name);
    printf("age: %d\n", stu1.age);
    printf("score: %d\n", stu1.score);

    return 0;
}
```

---