# midterm
midterm exam code and readme

url:https://github.com/RAJAHKOV/midterm 

软件包及版本：

### 1.Mingw g++ 8.1.0 

<img width="725" height="121" alt="image" src="https://github.com/user-attachments/assets/0273b5b2-6919-4431-85f4-d9b216856595" />

### 2.R 4.5.1

<img width="520" height="382" alt="image" src="https://github.com/user-attachments/assets/5d095279-0539-47bf-aa71-a08385cf31b5" />

### 3.Rtools45

<img width="817" height="265" alt="image" src="https://github.com/user-attachments/assets/58e905a0-9892-4e77-99ef-9c28f89e2498" />

### 4.Rcpp 1.1.2

<img width="240" height="41" alt="image" src="https://github.com/user-attachments/assets/959a73fe-473b-4fdd-b577-e4461a845b7a" />

### 5.RcppAmardillo 15.6.2.1

<img width="375" height="42" alt="image" src="https://github.com/user-attachments/assets/5f5f7b73-f2b0-4815-838c-694e5494cf1b" />


# A1.ode-solvers

编译命令:

```bash
g++ -std=c++11 ode-solvers.cpp -o ode-solvers.exe
```

运行命令:

```bash
.\ode-solvers.exe
```

运行结果:
```bash
h = 0.1, grid size = 21
Euler maximum absolute error: 0.241972
Improved Euler maximum absolute error: 0.0189048
h = 0.05, grid size = 41
Euler maximum absolute error: 0.127466
Improved Euler maximum absolute error: 0.00481986
```

本人已在课上完成且正确，因此未修改。验证方式是在更换文件位置之后再次编译运行程序，结果正确。

# A2.RandomNormalVector

编译命令：

```bash
g++ -std=c++11 random-normal-vector.cpp -o random-normal-vector.exe                       
```

运行命令:

```bash
.\random-normal-vector.exe
```

运行结果:
```bash
PASS: parameterized constructor
PASS: merge sort
PASS: mean
PASS: sample standard deviation
PASS: stream output
v1: -1.54681 -0.0249961 -1.54975 1.43654 -1.09458 1.26559 -1.48059 1.84105 -0.655247 -0.148124
v1 sorted: -1.54975 -1.54681 -1.48059 -1.09458 -0.655247 -0.148124 -0.0249961 1.26559 1.43654 1.84105
v2: -0.320222 1.96251 -0.324618 4.1548 0.358134 3.89838 -0.220886 4.76157 1.01713 1.77781
v2 mean: 1.70646, SD: 1.95629
PASS: Normal examples
```

本人已在课上完成且正确，因此未修改。验证方式是在更换文件random-normal-vector.cpp的地址之后再次编译运行程序，结果正确。

### A3.图像块平均降采样

运行命令:

```bash
source("block-pooling.R")
```

运行结果:
```bash
Small matrix, partial edge, identity and whole-image checks passed.
```

本人已在课上完成且正确，因此未修改。验证方式是在本地Visual Studio Code中再次运行block-pooling.R程序，结果正确。

### A4.加权最小二乘

运行命令:

```bash
source("weighted-least-squares.R")
```

运行结果:

```bash
$coefficients
[1] 0.9076389 0.9729167

$weighted_rss
[1] 0.6704861

R reference, all-one weights and rescaled-weight checks passed.
```

本人已在课上完成且正确，因此未修改。验证方式是在本地Visual Studio Code中再次运行weighted-least-squares.R程序，结果正确。

### A部分的AI使用情况

在课上做全程未使用任何AI工具 完成A3和A4是借助了[Rcpp教程](https://teuder.github.io/rcpp4everyone_en/index.html)和[RcppArmadillo文档](https://arma.sourceforge.net/docs.html)，其中参考了[uword的用法](https://arma.sourceforge.net/docs.html#uword),[qr_econ函数的参数](https://arma.sourceforge.net/docs.html#qr_econ)。
