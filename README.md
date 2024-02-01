<h1><div align="center"> Nonlinear equation params. estimation </div></h1>
<div align="left">

  
[![HTML](https://img.shields.io/badge/HTML-100000?style=flat&logo=html5&logoColor=red)](https://htmlpreview.github.io/?https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/.html/README.html)
</div>

<div align="right">
  
[![Jupyter](https://img.shields.io/badge/Notebook-000000?style=square&logo=jupyter&logoColor=orange)](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/nonlinear-eq_estimation.ipynb)</div>
</div>
<Details open>

<summary> <div style="font-family: Arial, sans-serif; color: #c4c8ff"> <b>Business Inquiries:</b> </div> </summary>

[<img width="40px" height="40px" src="https://img.icons8.com/ios/50/0e55b3/resume-website.png" alt="Resume">](https://estebanmqz.github.io/EstebanMqz/html/Resume.html)
[<img width="40px" height="40px" src="https://img.icons8.com/?size=512&amp;id=MR3dZdlA53te&amp;format=png" alt="LinkedIn">](https://www.linkedin.com/in/esteban-m65381722210212839/)
[<img width="36px" height="36px" src="https://cdn.worldvectorlogo.com/logos/whatsapp-business-bg.svg" alt="Business">](https://tinyurl.com/2y86e2wa)
<a href="mailto:emarquez1895@gmail.com" style="text-decoration: none;"><img width="40px" height="40px" style="max-width: 100%; max-height: 100%;" src="https://img.icons8.com/color/452/gmail-new.png" alt="Gmail"></a>
[<img width="40px" height="40px" style="max-width: 100%; max-height: 100%;" src="https://cdn3d.iconscout.com/3d/free/thumb/free-github-6343501-5220956.png?f=webp" alt="Github">](https://github.com/EstebanMqz?tab=repositories)
[<img width="40px" height="40px" style="max-width: 100%; max-height: 100%;" src="https://img.icons8.com/color/452/gitlab.png" alt="GitLab">](https://gitlab.com/EstebanMqz)


<div align= "left">
<div style="font-family: Arial, sans-serif; color: #c4c8ff; font-size: 18px;"> 

&#x26A1;Availability: <i> 24/7 on <b>WA</b> (business inquiries only) <br>
<div style="text-align: center;">
</b> <span style="color: #1b7521"> (password):</i> <b>"Marquez"</b></span><br></div>
</Details>
</div>

### Description:
From $n$ non-linear equations with $x_{1},..., x_n$ unknown variables a multivariate system of nonlinear equations with 
dimensional compatibility can be expressed: <br>

<div align="center"> <Details open> <Summary>  

###### <b>LaTeX parsed (Mobile):</b> </Summary>

![gh-app](images/Description.jpg)

</Details></div>

<b> The solution is found when the difference is 0 (10 iterations approx.)</b>
<br><br>

From [`Scipy: Non-linear solvers`](README.md#References) [`fsolve`](README.md#References) is used to estimate $f(x)$ distribution.<br>

The dataset <b>Cumulative Distribution</b> is:


$F(X)$ = ${Pr}(a \leq  X \leq b)$:

<font size="2"><i><b>Note:</b> Analytical tests should be performed to validate $f(x)$ & the obtained params $x_i,x_2,...,x_n:$</i></font>


$$F(X) = \int_{a}^{b} f(x) dx$$ 

$\therefore$ the <b>Expectancy</b> can be expressed as $E[Y]$:

$$E [Y] = \hat{F}^{N} = \int_{a}^{b} x f(x) dx$$ 

And $\hat{F}^{N}$ can be modelled with samplings from $N$ random variables $X \sim U(a,b)$.

<h3><a href="https://en.wikipedia.org/wiki/Beta_distribution">Beta Distribution</a></h3>

+ $X\sim\beta(\alpha, \beta)$ with $f(x_{i}, f_{x_{i}}):$ <br>

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

![Beta](images/Beta(x,a,b).png)<br><br>

<br>

<h3><a href="https://en.wikipedia.org/wiki/Triangular_distribution">Triangular Distribution</a></h3>

+ $X\sim\text{T}(a,b,c)$:

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

![Triang](images/Triang(x_c_a_b).png)<br><br>

+ Montecarlo Estimation:<br>

<div align="center"> <Details> <Summary>  

###### <b>LaTeX parsed (Mobile):</b> </Summary>

![gh-app](images/MC.jpg)

</Details></div>

<br>

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


<Details open>
<summary> <div style="font-family: Arial, sans-serif; color: #c4c8ff"> <i>Tools:</i> </div> </summary>


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

##### Repository: 

[![Repository](https://img.shields.io/badge/Repository-Visualization-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FNon-linear-eq-parameter-estimation-Samplings) 

<img src="images/diagram.svg" width="450"><br><br><br><br></div>
---
#### References: 

[`Non-Linear Solvers`](https://docs.scipy.org/doc/scipy/reference/optimize.html#id3)


[`Newton Raphson`](https://en.wikipedia.org/wiki/Newton%27s_method) [`Taylor-Series`](https://en.wikipedia.org/wiki/Taylor_series) [`Jacobian`](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)

[`scipy.optimize.fsolve`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fsolve.html)<br>

[`scipy.stats.beta`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.beta.html) $X\sim\beta(\alpha, \beta)$ <br>

[`scipy.stats.gamma`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gamma.html)
$X\sim\Gamma(\alpha, \beta)$ <br>

[`scipy.stats.triang`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.triang.html)
$X\sim\text{T}(a,b,c)$ 

[`Monte Carlo Estimation`](https://phyusdb.files.wordpress.com/2013/03/monte-carlo-methods-second-revised-and-enlarged-edition.pdf)



