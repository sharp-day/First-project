字符串变量初始化
#include <string.h>

char name[21];
memset(name,0,sizeof(name));
赋值
strcpy(name,"内容");



<h2>  常用库函数

int atoi(const char *name);    //把字符串name转换为int整数
int atol(const cahr *name);    //把字符串name转换为long整数
int abs(const int j);					//求int整数的绝对值
int labs(const long int j);			//求long整数的绝对值

void srand(unsigned int seed);		//随机数生成器的初始化函数
int rand();				//获一个取随机数
随机数一般用取余加法运算



```c
int isalpha(int ch);  // 若ch是字母（'A'-'Z','a'-'z'）返回非0值，否则返回0。
int isalnum(int ch);  // 若ch是字母（'A'-'Z','a'-'z'）或数字（'0'-'9'），返回非0值,否则返回0。
int isdigit(int ch);  // 若ch是数字（'0'-'9'）返回非0值，否则返回0。
int islower(int ch);  // 若ch是小写字母（'a'-'z'）返回非0值，否则返回0。
int isupper(int ch);  // 若ch是大写字母（'A'-'Z'）返回非0值，否则返回0。
int tolower(int ch);  // 若ch是大写字母（'A'-'Z'）返回相应的小写字母（'a'-'z'）。
int toupper(int ch);  // 若ch是小写字母（'a'-'z'）返回相应的大写字母（'A'-'Z'）
```



```c
double atof(const char *nptr);       // 把字符串nptr转换为double
double fabs(double x);                // 求双精度实数x的绝对值
double pow(double x, double y);      // 求 x 的 y 次幂（次方）
double round(double x);               // double四舍五入
double ceil(double x);                // double向上取整数
double floor(double x);               // double向下取整数
double fmod(double x,double y);      // 求x/y整除后的双精度余数
// 把双精度val分解成整数部分和小数部分，整数部分存放在ip所指的变量中，返回小数部分。
double modf(double val,double *ip);
```