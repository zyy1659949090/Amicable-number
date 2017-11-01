# Amicable-number

Amicable number

Problem Description

古希腊数学家毕达哥拉斯在自然数研究中发现，220的所有真约数(即不是自身的约数)之和为： 

1+2+4+5+10+11+20+22+44+55+110＝284。 


而284的所有真约数为1、2、4、71、 142，加起来恰好为220。人们对这样的数感到很惊奇，并称之为亲和数。一般地讲，如果两个数中任何一个数都是另一个数的真约数之和，则这两个数就是亲和数。 


你的任务就编写一个程序，判断给定的两个数是否是亲和数

 
Input

输入数据第一行包含一个数M，接下有M行，每行一个实例,包含两个整数A,B； 其中 0 <= A,B <= 600000 ; 


Output

对于每个测试实例，如果A和B是亲和数的话输出YES，否则输出NO。 


Sample Input

2

220 284

100 200 


Sample Output

YES

NO


解答：

#include<stdio.h>

main()

{

     double n,a,b,c,i;
     
     while(scanf("%lf",&n)!=EOF)
     
     {
     
      for(i=0;i<n;i++)
      
     {
     
     scanf("%lf%lf%lf",&a,&b,&c);
     
      if((a+b)>c&&(b+c)>a&&(a+c)>b)
      
      printf("YES\n");
      
      else
      
      printf("NO\n");
      
     }
     
     }
     
}    

