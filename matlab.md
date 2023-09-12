# Matlab基础

```matlab
readmatrix("");
xlsread("");
read();
```



# 方程

## 一般方程

```matlab
Example 4:%解方程组
   syms a u v;
   [Sa,Su,Sv] = solve(a*u^2 + v^2,u - v == 1,a^2 - 5*a + 6);

```

```matlab
s=solve(y*x==(x^2+10)*37.4/100,x);    %求解自变量为x的隐函数。
```

```matlab
Q1=a1*exp(-((x-b1)/c1)^2);
V1=int(Q1,0,0.45);                %求‘Q1’在0~0.45上的积分。
```



## 微分方程



# 数据处理

```matlab
1. yi = interpl(x,Y,xi)
2. yi = interpl(Y,xi)
3. yi = interpl(Y,xi,method)
临近点插值：method = 'nearest'
线性插值：method = 'linear'
三次样条插值：method = 'spline'
分段三次Hermite插值：method = 'pchip'
三次多项式插值：method = 'cubic'

%样条插值
1. yy = spline(x,y,xx)
2. pp = spline(xy)


[p,E] = polyfit(x,y,n);%多项式拟合
```



# 多元分析



# 绘图



# 数理统计

```matlab
A = randn(10,1);
B = randn(10,1);
R = corrcoef(A,B)%相关系数
```

聚类

```matlab
IDX=kmeans(all,2)
```
