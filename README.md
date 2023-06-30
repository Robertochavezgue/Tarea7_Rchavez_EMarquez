## **Non-linear-eq-params.-Estimators.**

#### **Repository Tools:**
<font>
<Details>
<Summary> <b>Click to expand</b> </Summary>

##### Actions:  [![Repo-Visualization-Badge](https://img.shields.io/badge/Action-Visualization-020521?style=square&logo=github&logoColor=white)](https://githubnext.com/projects/repo-visualization)<br>
##### Main Text-Editor:  [![VSCode-Badge](https://img.shields.io/badge/VSCode-007ACC?style=square&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/)  [![Jupyter-Badge](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=Jupyter&logoColor=white)](https://jupyter.org/try)<br>
##### Language:  [![Python-Badge](https://img.shields.io/badge/Python-2b6dd6.svg?style=square&logo=Python&logoColor=green)](https://www.python.org)  [![LaTeX-Badge](https://img.shields.io/badge/LaTeX-white.svg?style=square&logo=LaTeX&logoColor=008080)](https://www.latex-project.org)  [![Markdown-Badge](https://img.shields.io/badge/Markdown-000000.svg?style=square&logo=Markdown&logoColor=white)](https://www.markdownguide.org)  [![yaml-Badge](https://img.shields.io/badge/YAML-000000?style=square&logo=yaml&logoColor=red)](https://yaml.org)<br>
##### Libraries:[![Numpy-Badge](https://img.shields.io/badge/Numpy-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org)[![Pandas-Badge](https://img.shields.io/badge/Pandas-150458?style=square&logo=pandas&logoColor=white)](https://pandas.pydata.org)  [![Scipy-Badge](https://img.shields.io/badge/Scipy-darkblue?style=square&logo=scipy&logoColor=white)](https://www.scipy.org)  [![Matplotlib-Badge](https://img.shields.io/badge/Matplotlib-000000?style=flat-square&logo=Matplotlib&logoColor=white)](https://matplotlib.org)<br>
##### Web-Interface:&nbsp;[![React-Badge](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://create-react-app.dev)&nbsp;<br>
##### Version Control:&nbsp;[![GitHub-Badge](https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=github&logoColor=white)](https://github.com)&nbsp;[![Git-Badge](https://img.shields.io/badge/Git-F05032.svg?style=flat-square&logo=Git&logoColor=white)](https://git-scm.com)<br>
[![Git-Commads](https://img.shields.io/badge/Git%20Commands-gray?style=flat-square&logo=git&logoColor=white)](https://github.com/EstebanMqz/Git-Commands)<br><br>

##### License:&nbsp;[![Creative Commons BY 3.0](https://img.shields.io/badge/License-CC%20BY%203.0-yellow.svg?style=flat-square)](https://creativecommons.org/licenses/by/3.0/)<br>
</Details>

##### Work Contact: 
<font>
<Details>
<Summary> <b>Click to expand</b> </Summary>

[![Website](https://img.shields.io/badge/Website-ffffff?style=square&logo=opera&logoColor=red)](https://estebanmqz.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-041a80?style=square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/esteban-m65381722210212839/) [![Portfolio](https://img.shields.io/badge/Github-Portfolio-010b38?style=square&logo=github&logoColor=black)](https://estebanmqz.github.io/Portfolio/) [![E-mail](https://img.shields.io/badge/Business-Mail-052ce6?style=square&logo=mail&logoColor=white)](mailto:esteban@esteban.com)

![GitHub Logo](https://github.com/EstebanMqz.png?size=50) [![Github](https://img.shields.io/badge/Github-000000?style=square&logo=github&logoColor=white)](https://github.com/EstebanMqz)
</Details>

##### **Diagram:**
[![Repository](https://img.shields.io/badge/Repository-0089D6?style=square&logo=microsoft-azure&logoColor=white)](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=EstebanMqz%2FNon-linear-eq-parameter-estimation-Samplings)

<img src="diagram.svg" width="280" height="280"><br><br>

## **Description:**

![Alt text](images/Newton.jpg)

The main goal is to illustrate theoretically and practically the process on how to solve non-linear equations systems to estimate parameters for distributions $f(x)$, to obtain:<br>

$F(X)$ = ${Pr}(\{a \leq X \leq b\})$  $$F(X) = \int_{a}^{b} f(x) dx$$ <br>

And its expected value:

$$E [Y] = \hat{F}^{N} = \int_{a}^{b} x f(x) dx$$ 

Theoretically demonstrating $\hat{F}^{N}$ for $N$ random variables $x_{i} \in$ $[a,b] \sim U(a,b)$.

*Tests should be performed to validate the distribution and its parameters.*<br>

Afterwards Montecarlo (stratified) Samplings convergence speeds are compared between raw samplings and divided into $N$ strata.<br>

### **Results:**

+ For $x\sim\beta(\alpha, \beta)$ against $X\sim\beta$ prob. for data : <br>
$$x_{i_{\beta}}, f(x_{i_{\beta}})$$ <br>

<img src="/images/Beta.jpg" width="230" height="400">

<img src="/images/Beta(x,a,b).png" width="450" height="290">

<br>

+ For $x\sim\text{T}(a,b,c)$ with params $\alpha, \beta = a,b$ and $c_{(Mo)_{given}}$ <br>
compared against $X\sim\text{T}(a,b,c)$ accum. prob for data :

$$x_{i_{T}}, f(x_{i_{T}})$$ <br>

<img src="/images/triang.jpg" width="230" height="400">

<img src="/images/Triang(x,c,a,b).png" width="550" height="290"> <br>

+ Montecarlo Raw & Stratified Samplings:<br><br>

<img src="/images/MC_Samplings.png" width="375" height="250"> <br>


##### References: 
[`scipy.optimize.fsolve`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fsolve.html)<br>
[`scipy.stats.beta`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.beta.html)<br>
$x\sim\beta(\alpha, \beta)$<br>
[`scipy.stats.gamma`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gamma.html) <br>
$x\sim\Gamma(\alpha, \beta)$<br>
[`scipy.stats.triang`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.triang.html)<br>
$x\sim\text{T}(a,b,c)$



