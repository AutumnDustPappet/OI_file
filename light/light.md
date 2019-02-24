# 电灯 (light.cpp)

## 题目描述

有 $n$ 个灯泡排成一列。每个灯泡可能是点亮或熄灭的。有一台操控灯泡的机器，每一次可以选择一段区间，让这段区间中熄灭的灯泡全部点亮，亮着的灯泡全部熄灭。但由于机器已经老化，仅能再使用一次了。

你可以认为点亮的灯泡与熄灭的灯泡交替排列的样子（下面称这样的灯泡列为交替列）很好看。现在，你希望珍惜最后一次操控灯泡的机会，使得操控后这列灯泡中最长的交替列尽可能地长。

例如，这列灯泡若原本如下所示（○ 表示点亮的灯泡，● 为熄灭的灯泡）：
○ ○ ● ● ○ ● ○ ○ ○ ●

如果选择第 $4$ 个到第 $7$ 个灯泡，则会变成如下的形式：
○ ○ ● ○ ● ○ ● ○ ○ ●
此时，最长的交替列为第 $2$ 个到第 $8$ 个灯泡，长度为 $7$。

而如果仅选择第 $8$ 个灯泡，则会变成如下的形式：
○ ○ ● ● ○ ● ○ ● ○ ●
此时，最长的交替列为第 $4$ 个到第 $10$ 个灯泡，长度也为 $7$。

可以发现，此例中没有方法能使得最长交替列长度大于 $7$，则 $7$ 即为答案。

## 输入格式

输入文件第一行一个正整数 $n$，表示灯泡的数量。
第二行包含 $n$ 个数字，每个数字均为 0 或 1，依次代表序列中每个灯泡的初始状态。1 代表点亮，0 代表熄灭。

## 输出格式

输出一个整数，表示所有能得到的灯泡列中最长的交替列的长度。

## 样例输入

```text
10
1 1 0 0 1 0 1 1 1 0
```

## 样例输出

```text
7
```

## 数据规模与约定 

对于 $30\%$ 的数据，$1≤n≤500$。

对于 $60\%$ 的数据，$1≤n≤2000$。

对于 $100\%$ 的数据，$1≤n≤100000$。