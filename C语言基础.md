### 指针

例子1：

```c
int a =5; 
int *p;
p = &a;
```

指针p地址指向a



------



例子2：

```c
int a=5;
int *p = &a;
*p=4;
printf("%d,%d",*p,a);
```

- 指针指向a的地址；

  ==这部操作之后 *p和a的别名差不多。只不过可以操作地址==

- 修改指针指向地址的值，也就是修改a的值；



### 结构体

```c
#define MaxSize 100
typedef struct 变量名
{
    int data[MaxSize];
    int length;
}别名;
```

==c语言的结构体类似于java中的类的概念==



### 指针操作结构体内容

E1: 以顺序线性表为例为例

```c
typedef struct list{
    int data[100];
    int length;
}list；
list *l;
l->length=0;
list k;
k.length=0;

```

