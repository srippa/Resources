Resources
=========
**[Source control](#SRC) , [Languages and development tools](#LangIDEs), [IPython notebooks](#IPythonNotebook), [Numerical linear algebra](#LA)**


## <a id='SRC'></a>Source control
* I use [Git](http://git-scm.com/). Get started by browsing the [documentations](http://git-scm.com/doc). Also take a look at the [Curated Git links (2014)](http://thelinell.com/2014/12/23/curated-git-links-of-2014/) containing many pointers to useful resources. In particular I recommend to start by the  [how does Git work?](http://thelinell.com/2014/03/19/git/) post.
* I use [GitHub](https://github.com/) to store my pubic repositories.
* 

## <a id='LangIDEs'></a>Languages and development tools that I use

#### [C/C++](http://en.wikipedia.org/wiki/C%2B%2B)
* IDE, text editor, compiler: 
  * Windows - I usd [Visual Studio](http://www.visualstudio.com/en-us/products/free-developer-offers-vs.aspx#) which can be used free of charge for a single developer or a small team
  * Linux - I use the [gcc](https://gcc.gnu.org/) compiler
* Build language: I use [CMake](http://www.cmake.org/)


#### [R](http://www.r-project.org/)
R is the main statistical language with more than 5000 packages spanning nearly any topic in statistical computation. [RStudio](http://www.rstudio.com/) is the preferred IDE/text editor for the R language.
 

#### [Python](https://www.python.org/)
* The [Anaconda](https://store.continuum.io/cshop/anaconda/) distribution contains most of the packages needed for scientific computation. Uses the [conda](http://conda.pydata.org/docs/)  package manager. 
* Text editors/IDE
 * [Spyder](https://code.google.com/p/spyderlib/) is the Scientific PYthon Development EnviRonment -  Provided in the Anaconda distribution  
 * [SubLime Text](http://www.sublimetext.com/]) is a text editor for coding with syntax highlighting for many languages. Can be extended with plugins to be a descent substitution for a full fledged IDE, see Nathan Lemoine's post [My Ideal Python Setup for Statistical Computing](https://climateecology.wordpress.com/2014/11/26/my-ideal-python-setup-for-statistical-computing/) for ideas on how to turn SubLIme Text into a Python IDE
 * For fast prototyping and exploration I use [IPYthon notebook](#IPythonNotebook)

#### [Julia](http://julialang.org/)
THe Julia language is a relativly new language with the promise of the simplicity of Python and the performance of C/C++. This language is developing very fast and is worth of tracking. I use the IPYthon notebook based [IJulia](https://github.com/JuliaLang/IJulia.jl) environment for playing with the language.


## <a id='IPythonNotebook'></a>IPython notebook
[IPython notebooks](http://ipython.org/notebook.html) are a great for scientific exploration and for documentation of the work done. The IPython notebook allows mixing rich text with code sniplets. The text is written in a [markdown syntax](http://daringfireball.net/projects/markdown/) and HTML to produce a quite rich text format. IPython notebook uses [MathJax](http://www.mathjax.org/) to properly format mathematical formulas provided in [LaTeX](http://www.latex-project.org/) syntax. The official development environment supported by the notebook is [IPython](http://ipython.org/) which is focused on the [Python](https://www.python.org/) language. The flexible architecture of the IPython notebooks allows adding more languages such as [Julia](https://github.com/JuliaLang/IJulia.jl), [R](http://rpy.sourceforge.net/rpy2/doc-2.4/html/interactive.html#module-rpy2.ipython.rmagic) and others.

It is possible to share public notebooks using a [notebooks viewer service](http://nbviewer.ipython.org/) which renders the notebook as a static HTML file tat can be displayed to any client with a browser. A growing collections of [interesting notebooks](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks) cover many interesting topics. The notebook viewer is particularly useful to view public notebooks stored in GitHub. You can make a connection to the notebooks managed by GitHub and the most recent version will be displayed in the notebook viewer. This allows any client with a browser to view your notebooks.

In most cases storing IPython notebooks within a version control like Git works well. The [problem is](http://stackoverflow.com/questions/18734739/using-ipython-notebooks-under-version-control?rq=1) that sometimes the standard notebook file (with the extension **.ipynb**) contains also the output of computational procedures such as, for example,  plotting or images displayed. Those are reresented as binary blobs that may occupy a lot of space. The problem and some remedies are discussed [in this StackOverflow discussion](http://stackoverflow.com/questions/18734739/using-ipython-notebooks-under-version-control?rq=1)

**Some relevant notebooks**
* [Using Git](http://nbviewer.ipython.org/github/demotu/BMC/blob/master/notebooks/VersionControlGitGitHub.ipynb)
* [Notebook tricks for scientific computing](http://nbviewer.ipython.org/github/NelisW/ComputationalRadiometry/blob/master/01-IPythonHintsAndTips.ipynb)


##  <a id='LA'></a> Numerical linear algebra
Linear algebra is a central infrastructure driving scientific computation in general and more specifically data science and machine learning solutions. 

### Books
  * [Introduction to Linear Algebra](http://www.amazon.com/dp/0980232716?tag=inspiredalgor-20) by Gilbert Strang.
  * [Matrix Computation](http://www.amazon.com/dp/1421407949?tag=inspiredalgor-20) by Gene Golub and Charles Van Loan.

### Courses and Videos
  * [Video lectures of Professor Gilbert Strang](http://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/).

### Software
  * [BLAS](http://www.netlib.org/blas/)/[LAPACK](http://www.netlib.org/lapack/) are the de facto standards for the language of numerical linear algebra. The libraries are written in FORTRAN but can be linked with any high level language
  * C++
    * [Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page)
    * [Armadillo](http://arma.sourceforge.net/)
  * Python
    * The main data structure for n-dimensional arrays is given by [numpy](http://docs.scipy.org/doc/numpy/reference/), more specific linera algebra procedures are in the [linear algebra module](http://docs.scipy.org/doc/numpy/reference/routines.linalg.html)
