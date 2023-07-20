## **Nonlinear equation params. estimation**

<Details>
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

<Details>

<a name ="repo-visualization"></a>

<Summary> <i>Repo Visualization:</i> </Summary>

[![Repository](https://img.shields.io/badge/Repository-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FNon-linear-eq-parameter-estimation-Samplings)

<img src="diagram.svg" width="280" height="280"><br><br>

</Details>

<div align="right">
<Details>
<Summary> <i>Contact:</i> </Summary>

[![Website](https://img.shields.io/badge/Website-ffffff?style=square&logo=opera&logoColor=red)](https://estebanmqz.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-041a80?style=square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/esteban-m65381722210212839/) [![Portfolio](https://img.shields.io/badge/Github-Portfolio-010b38?style=square&logo=github&logoColor=black)](https://estebanmqz.github.io/Portfolio/) [![E-mail](https://img.shields.io/badge/Business-Mail-052ce6?style=square&logo=mail&logoColor=white)](mailto:esteban@esteban.com)

![GitHub Logo](https://github.com/EstebanMqz.png?size=50) [![Github](https://img.shields.io/badge/Github-000000?style=square&logo=github&logoColor=white)](https://github.com/EstebanMqz)

</Details></div>

---

## **Description:**

![Description](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/Description.jpg)


Using [`fsolve`](#README.md#References) to solve for non-linear equations systems to estimate params. for distributions $f(x)$, to obtain:

$F(X)$ = ${Pr}(a \leq X \leq b)$:

<i>Analytical tests should be performed to validate $f(x)$ $\&$ the obtained params:</i>


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

![MC](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/MC.jpg)<br>

<i>(See [Nbrender]())</i>
![Samplings](https://github.com/EstebanMqz/Non-linear-equation-Parameter-estimation/blob/main/images/MC_Samplings.png)


##### References: 
[`Newton Raphson`](https://en.wikipedia.org/wiki/Newton%27s_method) [`Taylor-Series`](https://en.wikipedia.org/wiki/Taylor_series) [`Jacobian`](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)

[`scipy.optimize.fsolve`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fsolve.html)<br>

$X\sim\beta(\alpha, \beta)$ [`scipy.stats.beta`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.beta.html)<br>

$X\sim\Gamma(\alpha, \beta)$ [`scipy.stats.gamma`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gamma.html)<br>

$X\sim\text{T}(a,b,c)$ [`scipy.stats.triang`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.triang.html)

[`Monte Carlo Estimation`](https://phyusdb.files.wordpress.com/2013/03/monte-carlo-methods-second-revised-and-enlarged-edition.pdf)
