<h1><div align="center"> Nonlinear equation params. estimation </div></h1>

<Details Open>
<Summary> <i>Tools:</i> </Summary>

##### Actions:  [![Repo-Visualization-Badge](https://img.shields.io/badge/Action-Visualization-020521?style=square&logo=github&logoColor=white)](https://githubnext.com/projects/repo-visualization)<br>
##### Main Text-Editor:  [![VSCode-Badge](https://img.shields.io/badge/VSCode-007ACC?style=square&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/)  [![Jupyter-Badge](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=Jupyter&logoColor=white)](https://jupyter.org/try)<br>
##### Language:  [![Python-Badge](https://img.shields.io/badge/Python-2b6dd6.svg?style=square&logo=Python&logoColor=green)](https://www.python.org)  [![LaTeX-Badge](https://img.shields.io/badge/LaTeX-white.svg?style=square&logo=LaTeX&logoColor=008080)](https://www.latex-project.org)  [![Markdown-Badge](https://img.shields.io/badge/Markdown-000000.svg?style=square&logo=Markdown&logoColor=white)](https://www.markdownguide.org)  [![yaml-Badge](https://img.shields.io/badge/YAML-000000?style=square&logo=yaml&logoColor=red)](https://yaml.org)<br>
##### Libraries:[![Numpy-Badge](https://img.shields.io/badge/Numpy-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org)[![Pandas-Badge](https://img.shields.io/badge/Pandas-150458?style=square&logo=pandas&logoColor=white)](https://pandas.pydata.org)  [![Scipy-Badge](https://img.shields.io/badge/Scipy-darkblue?style=square&logo=scipy&logoColor=white)](https://www.scipy.org)  [![Matplotlib-Badge](https://img.shields.io/badge/Matplotlib-000000?style=flat-square&logo=Matplotlib&logoColor=white)](https://matplotlib.org)<br>
##### Web-Interface:&nbsp;[![React-Badge](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://create-react-app.dev)&nbsp;<br>
##### Version Control:&nbsp;[![GitHub-Badge](https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=github&logoColor=white)](https://github.com)&nbsp;[![Git-Badge](https://img.shields.io/badge/Git-F05032.svg?style=flat-square&logo=Git&logoColor=white)](https://git-scm.com)<br>
[![Git-Commands](https://img.shields.io/badge/Git%20Commands-gray?style=flat-square&logo=git&logoColor=white)](https://github.com/EstebanMqz/Git-Commands)<br><br>

##### License:&nbsp;[![Creative Commons BY 3.0](https://img.shields.io/badge/License-CC%20BY%203.0-yellow.svg?style=flat-square)](https://creativecommons.org/licenses/by/3.0/)<br>
</Details>

<div align="center">
  
<Details Open>  
<Summary> <i>Repo Visualization:</i> </Summary>
  
[![Repository](https://img.shields.io/badge/Repository-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FNon-linear-eq-parameter-estimation-Samplings) [![Jupyter](https://img.shields.io/badge/Render-nbviewer-000000?style=square&logo=jupyter&logoColor=orange)](https://nbviewer.org/github/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/nonlinear-eq_estimation.ipynb)

<a name ="repo-visualization"></a>
<img src="diagram.svg" width="280" height="280"><br><br>

</Details> </div>

<div align="right">
<Details open>
<Summary> <i>Business Inquiries:</i> </Summary>

[<img width="40px" src="https://img.icons8.com/ios/50/0e55b3/resume-website.png">](https://estebanmqz.github.io/EstebanMqz/html/Resume.html)
[<img width="40px" src="https://img.icons8.com/?size=512&id=MR3dZdlA53te&format=png">](https://www.linkedin.com/in/esteban-m-653817205/)
[<img width="35px" src="https://img.icons8.com/color/452/whatsapp--v1.png">](https://tinyurl.com/2y86e2wa)
[<img width="40px" src="https://img.icons8.com/color/452/gmail-new.png">](mailto:emarquez1895@gmail.com)
[<img width="40px" src="https://cdn3d.iconscout.com/3d/free/thumb/free-github-6343501-5220956.png?f=webp">](https://github.com/EstebanMqz?tab=repositories)
[<img width="40px" src="https://img.icons8.com/color/452/gitlab.png">](https://gitlab.com/EstebanMqz)

</Details></div>

<b> Job-Related Meetings through LinkedIn:</b><br>
<i>Connect with me if you need my assistance 24/7 to be alert on WA-Business (pw required).</i>
<br><br>

---

## **Description:**

From $n$ non-linear equations with $x_{1},..., x_n$ unknown variables a multivariate system of nonlinear equations with 
dimensional compatibility can be expressed: <br>

[gh-app](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/Description.jpg)

<div class="alert alert-block alert-info">

$f_1(x_1,x_2,...,x_n) = 0$ <br>
$f_2(x_1,x_2,...,x_n) = 0$ <br>
$\vdots$ <br>
$f_n(x_1,x_2,...,x_n) = 0$ <br>

A common method of approximatation for the solutions of $x_1,x_2,...,x_n$ is [Newthon's](README.md#References) method with the roots of terms ${ }_{1,2}$ of the [Taylor series](README.md#References) expansion:<br>
$f(x) = f(x_n) + f'(x_n)(x-x_n) + \frac{f''(x_n)}{2!}(x-x_n)^2 +\cdots + \frac{f^{n}(x_n)}{n!}(x-x_n)^n$ = 0<br>
$f(x) = f(x_n) + f'(x_n)(x-x_n) = 0$ <br>

Generalizing for $n$ variables, we have: <br>
$x_{n+1} = x_n - \frac{f(x_i)}{f'(x_i)} = x_n - J(x)^{-1} \cdot f(x_i)$ <br>

The [Jacobian](README.md#References) matrix is obtained by taking the first derivative of each function with respect to each variable. <br>

$$
J(x) = \begin{bmatrix}
\frac{\partial f_1}{\partial x_1} & \frac{\partial f_1}{\partial x_2} & \cdots & \frac{\partial f_1}{\partial x_n} \\
\frac{\partial f_2}{\partial x_1} & \frac{\partial f_2}{\partial x_2} & \cdots & \frac{\partial f_2}{\partial x_n} \\
\vdots & \vdots & \ddots & \vdots \\
\frac{\partial f_n}{\partial x_1} & \frac{\partial f_n}{\partial x_2} & \cdots & \frac{\partial f_n}{\partial x_n} \\
\end{bmatrix}
$$

$\therefore$ the equation is rewritten with $x_n$ and $f(x_i)$ as vectors evaluated in $x_n$:<br> 
$x_n = [x_1, x_2, ..., x_n]^T$ <br>
$f(x_i) = [f_1(x_1,x_2,...,x_n)$, $f_2(x_1,x_2,...,x_n)$, $\cdots$ , $f_n(x_1,x_2,...,x_n)]^T$<br>

So iteration $1$ of a Newton-Raphson method is constructed for a multivariate system of nonlinear equations:<br>
  
<div align="right">

<i> (see [refs.](README.md#Referencess) for more info.) </i> 
</div>

<i> The solution is found when $|x_{n+1} \pm x_n| \approx 0$. </i>
<br><br>

Using [`fsolve`](README.md#References) to solve for non-linear equations systems to estimate params. for distributions $f(x)$, to obtain:

$F(X)$ = ${Pr}(a \leq X \leq b)$:

<i>Analytical tests should be performed to validate $f(x)$ & the obtained params:</i>


$$F(X) = \int_{a}^{b} f(x) dx$$ 

$\therefore$ Obtain the expectancy $E[Y]$:

$$E [Y] = \hat{F}^{N} = \int_{a}^{b} x f(x) dx$$ 

Where $\hat{F}^{N}$ can be modelled with samplings from $N$ random variables $X \sim U(a,b)$.

### **Results:**

+ For $X\sim\beta(\alpha, \beta)$ for data $f(x_{i}, f_{x_{i}}):$ <br>

|   x   |   f(x)   |   F(x)   |
|-------|---------|---------|
| 40.00 |   inf   | 0.000000|
| 40.01 | 1.040696| 0.019154|
| 40.02 | 0.758528| 0.027915|
| 40.03 | 0.630507| 0.034797|
| 40.04 | 0.553063| 0.040688|
|  ...  |   ...   |   ...   |
| 48.95 | 0.247013| 0.981838|
| 48.96 | 0.265219| 0.984395|
| 48.97 | 0.290729| 0.987167|
| 48.98 | 0.330971| 0.990257|
| 48.99 | 0.413234| 0.993916|

![Beta](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/Beta(x%2Ca%2Cb).png)

<br>

+ For $X\sim\text{T}(a,b,c)$:

|   x   |   f(x)   |   F(x)   |
|-------|---------|---------|
|  0    | 40.000000| 0.000000|
|  1    | 40.090909| 0.005102|
|  2    | 40.181818| 0.010203|
|  3    | 40.272727| 0.015305|
|  4    | 40.363636| 0.020406|
|  ...  |   ...   |   ...   |
|  95   | 48.636364| 0.997085|
|  96   | 48.727273| 0.998360|
|  97   | 48.818182| 0.999271|
|  98   | 48.909091| 0.999818|
|  99   | 49.000000| 1.000000|

![Triang](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/Triang(x%2Cc%2Ca%2Cb).png)<br><br>

+ Montecarlo Estimation:<br>

[gh-app](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/MC.jpg)<br>

<div class="alert alert-block alert-info">

if $V$ is the volume of an integral 

$$V = \int_{a}^{b} f(x) dx$$
   
and it follows a uniform prob. density function $f(x)$ $X \sim U(a,b)$ it can be modelled with `np.random.uniform`.<br>

$f(x) = \frac{1}{b-a}$ if $a \leq x \leq b$ <br>
$0$ otherwise

<i>Nevertheless if the distribution isn't known it must be obtained from data or modelled with another method.</i>

From where we've got by the definition the expectancy:<br>

$$E[X] = \int_{a}^{b} x f(x) dx$$

Then, the mean of $x_{i}$ in $V$ is:

$$F = \frac{V}{N} \sum_{i=0}^{N-1} f\left(x_i\right)$$

if $N = N-1$ the equation can be rewritten from the solution of the integral as:
$$F = \frac{b-a}{N-1} \sum_{i=0}^N f\left(x_i\right)$$

But Montecarlo estimations for $N$ random variables $X \sim U(a,b)$ must include the error  $\xi$.<br>
$\therefore$, the estimator can be expressed with the solution of the integral for all possible errors $\xi \in$ $(0,1]$ $\rightarrow$ $a = b$ :

$$\hat{F}^{N} = \frac{b-a}{N-1} \sum_{i=0}^{N} f\bigg[a + \xi(b-a)\bigg]$$

![Samplings](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/MC_Samplings.png)

<div align="right">

<i>(see [nbrender](README.md#Repo-Visualization) for more details.)</i><br>

</div>

##### References: 
[`Newton Raphson`](https://en.wikipedia.org/wiki/Newton%27s_method) [`Taylor-Series`](https://en.wikipedia.org/wiki/Taylor_series) [`Jacobian`](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)

[`scipy.optimize.fsolve`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fsolve.html)<br>

$X\sim\beta(\alpha, \beta)$ [`scipy.stats.beta`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.beta.html)<br>

$X\sim\Gamma(\alpha, \beta)$ [`scipy.stats.gamma`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gamma.html)<br>

$X\sim\text{T}(a,b,c)$ [`scipy.stats.triang`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.triang.html)

[`Monte Carlo Estimation`](https://phyusdb.files.wordpress.com/2013/03/monte-carlo-methods-second-revised-and-enlarged-edition.pdf)
