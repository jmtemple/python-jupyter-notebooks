# Python and Jupyter Notebooks

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Goals

By the end of this tutorial, students will be able to:
- Install Anaconda in their local environment
- Understand the core components of the Jupyter Notebooks environment

## Acknowledgements

The documentation for Google Colab was developed by Spring 2021 graduate teaching assistant [Subhadyuti Sahoo](https://github.com/SDSAHOO703).

Peer review and editing was provided by Spring 2021 graduate teaching assistants [Subhadyuti Sahoo](https://github.com/SDSAHOO703) and [Aidan Draper](https://github.com/adraper2).

The author consulted the following texts when writing this tutorial:
- Allen Downey, [*Think Python: How to Think Like a Computer Scientist*](https://www.oreilly.com/library/view/think-python-2nd/9781491939406/) (O'Reilly, 2015).
  * Chapter 2 "Variables, Expressions and Statements" (11-20)
- Quinn Dombrowski, Tassie Gniady, and David Kloster, "Introduction to Jupyter Notebooks," *The Programming Historian* 8 (2019), https://doi.org/10.46430/phen0087

# Table of Contents

- [Different types of Python environments](#different-types-of-python-environments)
- [Installing Anaconda](#installing-anaconda)
- [Python in Jupyter notebooks](#python-in-jupyter-notebooks)
  * [Installing packages in Jupyter notebooks](#installing-packages-in-jupyter-notebooks)
  * [Authoring in Jupyter notebooks](#authoring-in-juyter-notebooks)
  * [Jupyter notebook export options](#jupyter-notebook-export-options)
- [IF NEEDED: Getting Started With Google CoLab](#getting-started-with-google-colab)
- [Other Lab Notebook Questions](#other-lab-notebook-questions)
- [OPTIONAL: Python in Spyder](#optional-python-in-spyder)
- [Lab Notebook Questions](#lab-notebook-questions)


# Different types of Python environments

What is an IDE? "An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger" ([Wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)).

An IDE can include features like syntax highlighting, code completion, version control, and debugging.

There are a WIDE range of IDEs that are proprietary or open-source, tailored to a specific language or able to work across languages.

Some common IDEs include Eclipse, Geany, Brackets, Atom, PyCharm, Spyder, RStudio, etc. For more in IDEs, visit Wikipedia's ["Comparison of integrated development environments"](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments) page.

 

Now, we're going to install Python on your local computer, using a distribution called Anaconda.

What is Anaconda? "Anaconda is a open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012" ([Wikipedia](https://en.wikipedia.org/wiki/Anaconda_(Python_distribution))).

The Anaconda environment includes a number of specific tools and programs, including:
- JupyterLab
- Jupyter Notebook
- Qt Console
- Spyder
- Glue
- Orange
- RStudio
- Visual Code Studio

This tutorial introduces us to using Jupyter Notebooks through Anaconda. It also includes resources for [getting started in Google Colab](https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/google-colab-instructions.md), a browser-based Jupyter Notebooks environment.

# Installing Anaconda

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

Windows/PC instructions:
- Anaconda Documentation, ["Installing on Windows"](https://docs.anaconda.com/anaconda/install/windows/) *Anaconda* (2020).
- ProgrammingKnowledge, ["Install Anaconda Python, Jupyter Notebook and Spyder on Windows 10"](https://youtu.be/5mDYijMfSzs) *YouTube video* (4 September 2018).

Mac OS instructions:
- Anaconda Documentation, ["Installing on macOS"](https://docs.anaconda.com/anaconda/install/mac-os/) *Anaconda* (2020).
- Understanding Data, ["Easily Install Anaconda Python Distribution On Mac OS X"](https://youtu.be/V6ZAv7hBH6Y) *YouTube video* (16 October 2019).

Chromebook instructions:
- Alex P. Miller, ["Data Science on a Chromebook: How to run Jupyter, Python, and R locally in ChromeOS"](https://alex.miller.im/posts/data-science-chromebook-pixelbook-jupyter-python-r/) *personal blog* (6 March 2019).
- Noebrian, ["Installing Anaconda on a Chromebook"](https://chromebook.home.blog/2019/01/20/installing-anaconda-on-a-chromebook-no-dev-beta-or-crouton-needed/) *ChromeBooks* (20 January 2019).

# Python in Jupyter notebooks

What is Jupyter?

"Project Jupyter is a non-profit, open-source project, born out of the IPython Project in 2014 as it evolved to support interactive data science and scientific computing across all programming languages. Jupyter will always be 100% open-source software, free for all to use and released under the liberal terms of the modified BSD license" (["About Us"](https://jupyter.org/about), *Jupyter.org*)

Project Jupyter receives funding from a range of non-profit foundations and corporate partners that include:
- Alfred P. Sloan Foundation
- Gordon and Betty Moore Foundation
- Google
- Microsoft

Institutional partners for Project Jupyter include:
- Apple
- Bloomberg
- Netflix
- Cal Poly
- Berkeley
- Amazon Web Services (AWS)

The name Jupyter is a reference to the three core languages supported by the project: **Ju**lia, **Py**thon, and **R**.

And what is a Jupyter notebook?

According to "[The Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html)" documentation:

<blockquote>The notebook extends the console-based approach to interactive computing in a qualitatively new direction, providing a web-based application suitable for capturing the whole computation process: developing, documenting, and executing code, as well as communicating the results. The Jupyter notebook combines two components:
 <ul>
  <li>A web application: a browser-based tool for interactive authoring of documents which combine explanatory text, mathematics, computations and their rich media output.</li>
  <li>Notebook documents: a representation of all content visible in the web application, including inputs and outputs of the computations, explanatory text, mathematics, images, and rich media representations of objects</li>
 </ul>
 </blockquote>

A Jupyter notebook is a file (the notebook document) that displays or renders in a web browser.

We'll be launching Jupyter Notebooks through Anaconda. 

The web application component of the notebook will be hosted on your local computer and the notebook document will save to a file directory on your local computer.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_5.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_5.png?raw=true" /></a></p>

It may take some time for the notebook to open in a browser window.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_6.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_6.png?raw=true" /></a></p>

When in a new notebook document, you have four main components to the user interface:
- Notebook name
- Menu bar
- Toolbar
- Code cell

The notebook name is what the `.ipynb` file created via the Jupyter notebook will be saved as.

Click on the default notebook name (usually `Untitled`) to rename the notebook. You will name your lab notebooks as follows: Lab#_Notebook_Templeton.ipynb. 

The menu bar includes drop-down options used to manipulate the notebook functionality.

The toolbar icons give you quick access to the most commonly-used features of the notebook environment.

Code cells are the default type of cell.

But why are there cells?

Jupyter notebooks consist of a sequence of cells.

A cell is a multiline text input field. 

You can execute the contents of a cell by using `Shift-Enter`, clicking the `Play` button in the toolbar, or the `Cell` and `Run` icons in the menu bar.

How a cell executes is determined by its type.

There are three types of Jupyter notebook cells.

***Code cells*** allow you to edit and write code with full syntax highlighting and tab completion.

***Markdown cells*** allow you to document the computational process using descriptive text formatted using the markdown language.

***Raw cells*** allow you to write output directly. These cells are not evaluated by the notebook and render unmodified.

You can edit or work within a code cell until you get the desired output, then move on to a new cell.

You can use markdown cells along the way to document your process using narrative text (alongside or in addition to code comments used in code cells).

To learn more about formatting text in markdown, visit Adam Pritchard's ["Markdown Cheatsheet"](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) resource page.

You can download a Jupyter notebook as a `.ipynb` file (this is the default option).

You can also use the `File` - `Download as` menu options to download the notebook in a number of other formats, including `.py`, `.pdf`, or `.html`.

<blockquote>To learn more about configuring Jupyter Notebooks to download notebooks as PDFs:
 <ul>
  <li><a href="https://pypi.org/project/notebook-as-pdf/">Jupyter extension documentation</a></li>
  <li>Cornellius Yudha Wijaya, "<a href="https://towardsdatascience.com/jupyter-notebook-to-pdf-in-a-few-lines-3c48d68a7a63">Jupyter Notebook to PDF in a few lines</a>", <em>Towards Data Science</em> (12 July 2020)</li>
 </ul>
 </blockquote>

There's a lot to love about Jupyter notebooks. 

A few challenges or drawbacks:
- Version control especially in collaborative environments is virtually impossible
- Jupyter lacks the debugging tools and autocompletion features of an IDE
- Installing third-party packages or modules can be tricky 
- Jupyter's non-linear workflow limits transparent reproducible code
- Jupyter doesn't play well with external big data applications (spark/dask/distributed)

<blockquote>Citation: Alexander Mueller, <a href= "https://towardsdatascience.com/5-reasons-why-jupyter-notebooks-suck-4dc201e27086">"5 reasons why jupyter notebooks suck"</a>, <i>Towards Data Science</i> (24 March 2018)</blockquote>

So when could you use Jupyter notebooks? 

Jupyter notebooks are fantastic tools for exploration. 

They also work well for documenting process, or in situations when you might need to alternate between code and other kinds of text (like say in a lab notebook).

### Installing packages in Jupyter notebooks

In some labs, you can / will need to use modules, libraries, and packages to extend Python's functionality.

These include `csv` and `json` modules for example.

There are many situations in which we would need to install a Python module, package, or library before being able to use `import` as shown below.

```Python
# sample import statement
import MODULE NAME
```

Let's take a look at the installation instructions for a few common Python libraries.
- `NumPy` (scientific computing), ["Installing NumPy"](https://numpy.org/install/)
- `SciKit-Learn` (machine learning), ["Installing scikit-learn"](https://scikit-learn.org/stable/install.html)
- `pandas` (data wrangling/analysis) ["Installation"](https://pandas.pydata.org/docs/getting_started/install.html)
- `matplotlib` (data visualization) ["Installation"](https://matplotlib.org/stable/users/installing.html)

The documentation for each library includes sample code for installing the library in different Python environments and operating systems.

Many libraries/packages will include sample code for installing the package using `pip`, an installation method available through the Python Package Index.

Most libraries/packages will also include sample code for installing the package through Anaconda, sometimes referred to as `conda` in documentation.

BUT...these install commands are not something we should run within our Python program, whether we're working in a `.py` script or a `.ipynb` notebook.

You might see internet documentation that suggests you apply the install terminal syntax directly in a code cell.

```Python
!conda install --yes numpy

!pip install numpy
```

Resist this temptation!

We want to make sure the library is installed correctly in our Python environment, so we need to run the install command in a terminal/shell.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig4.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig4.jpg?raw=true" /></a></p>

You can access a terminal/shell by launching the Anaconda Navigator and clicking the `Launch` button in the `CMD.exe Prompt` tile.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig5.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig5.jpg?raw=true" /></a></p>

Then, within the terminal, we can run the install command.
- `pip` will work, but when possible `conda` is best

We can also open a terminal from within Jupyter Notebooks.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig1.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig1.jpg?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig2.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig2.jpg?raw=true" /></a></p>

In the Jupyter Notebook main window (first browser tab that opens when you launch the program), click the `New` drop-down in the top right-hand corner.

Select `Terminal` under `Other` to open a terminal.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig3.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig3.jpg?raw=true" /></a></p>

Then, within the terminal, we can run the install command.
- Again, `pip` will work, but when possible `conda` is best.

If you absolutely must install a package from within a notebook, we can use the `sys` module to install the package from within the notebook.

```Python
# sample code for installing numpy using conda

# import sys module
import sys

# line of code to install numpy using conda
!conda install --yes --prefix {sys.prefix} numpy
```

```Python
# sample code for installing numpy using pip

# import sys module
import sys

# line of code to install numpy using pip
!{sys.executable} -m pip install numpy
```

For more on installing Python packages in the Jupyter notebook environment:
- Jake VanderPlas, ["Installing Python Packages from a Jupyter Notebook"](https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/) *Pythonic Perambulations personal blog* (5 December 2017)

If you have already installed a package at the command line using `pip` or `conda`, launching Jupyter from the Anaconda navigator should not require installing the package again.

<blockquote>Q1: Use the Anaconda or Jupyter terminal to install the four libraries mentioned in step 55 (numpy, scikit-learn, pandas, matplotlib). Describe your experience installing these libraries using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?</blockquote>

You can load the module/library/package in your Python program using `import`.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/module_error.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/module_error.png?raw=true" /></a></p>

The `import` statements won't have an output, but the absence of a `ModuleNotFoundError` message is a good sign.

<blockquote>Q2: Write import statements for each of the libraries you installed in Q1. What did you expect to happen? What challenges did you face (if any)?</blockquote>

```Python
# import pandas 
import pandas

# import pandas using pd alias
import pandas as pd
```

```Python
# import numpy
import numpy

# import numpy using np alias
import numpy as np
```

```Python
# import scikit-learn
import sklearn

# import datasets module from scikit-learn
from sklearn import datasets

# import linear models from scikit-learn
from sklearn import linear_model
```

```Python
# import matplotlib
import matplotlib.pyplot

# import matplotlib using plt alias
import matplotlib.pyplot as plt
```

## Authoring in Jupyter Notebooks

Remember there are three types of Jupyter notebook cells.
- ***Code cells*** allow you to edit and write code with full syntax highlighting and tab completion.
- ***Markdown cells*** allow you to document the computational process using descriptive text formatted using the markdown language.
- ***Raw cells*** allow you to write output directly. These cells are not evaluated by the notebook and render unmodified.

There are a few ways you can change a cell's type.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig6.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig6.jpg?raw=true" /></a></p>

One option is to select the cell type from the drop-down options.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig7.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig7.jpg?raw=true" /></a></p>

Another option is to select `Cell Type` from the `Cell` menu tab.

You'll also notice there are keyboard shortcuts for changing cell type.
- `y` (code)
- `m` (markdown)
- `r` (raw)

A couple of notes on keyboard shortcuts...
- When a cell is highlighted in green (click inside the cell's text box), this indicates you are editing in the cell.
- When a cell is highlighted in blue (click to the left of the cell's text box), this indicates you are modifying the entire cell.

A few other useful keyboard shortcuts:
- `x` (delete a cell)
- `a` (insert cell above, default is code cell)
- `b` (insert cell below, default is code cell)

To put that another way:
- Green: Typing code, adding text to a markdown cell, etc.
- Blue: Changing the type of cell using keyboard shortcuts

<blockquote>Q3: In a markdown cell, add text that includes the following style or formatting components:
 <ul>
  <li>Heading (h1, h2, h3, etc)</li>
  <li>Italics or bold text formatting</li>
  <li>Unordered (or bulleted point) list</li>
  <li>Link</li>
 </ul>
 NOTE: You will want to reference Adam Pritchard's <a href="https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet">Markdown Cheatsheet</a> resource when working on this question.
 </blockquote>

<blockquote>Q4: In a code cell, write a simple Python program (or programs) that includes the following functions:
 <ul>
  <li><code>input()</code></li>
  <li><code>print()</code></li>
 </ul>
 You are welcome to use a program (or programs) you've written for previous labs- original code is not required for this question. The main point for this question is to see how a Jupyter Notebook code cell executes a program.</blockquote>
 
## Jupyter Notebook Export Options

You can download a Jupyter notebook as a `.ipynb` file (this is the default option).

You can also use the `File` - `Download as` menu options to download the notebook in a number of other formats, including `.py`, `.pdf`, or `.html`.

NOTE: The PDF export options require additional configuration.

Specifically, we're going to install the `notebook-as-pdf` and `pyppeteer` libraries. These allow HTML and PDF export and are much easier than trying to set up and configure LaTeX.

Open a terminal (through Anaconda or Jupyter) and type the following commands (hitting `Enter` or `Return` after each line).

```
python -m pip install -U notebook-as-pdf
pyppeteer-install
```

Once both installation processes have completed, you can close the terminal.

You will need to restart the Python Kernel for the new export options to be available.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig8.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig8.jpg?raw=true" /></a></p>

Click one of the `Restart` options under the `Kernel` menu tab.

If needed, re-run any code cells.

<blockquote>To learn more about configuring Jupyter Notebooks to download notebooks as PDFs:
 <ul>
  <li><a href="https://pypi.org/project/notebook-as-pdf/">Jupyter extension documentation</a></li>
  <li>Cornellius Yudha Wijaya, "<a href="https://towardsdatascience.com/jupyter-notebook-to-pdf-in-a-few-lines-3c48d68a7a63">Jupyter Notebook to PDF in a few lines</a>", <em>Towards Data Science</em> (12 July 2020)</li>
 </ul>
 </blockquote>

# Getting Started With Google CoLab

Anaconda is a hefty software program that may not run (or run well) on your personal computer.

"'Colaboratory,' or 'CoLab' for short, is a product from Google Research. Colab allows anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs." ([Google Colaboratory, "Frequently Asked Questions"](https://research.google.com/colaboratory/faq.html))

If Jupyter Notebooks through Anaconda is not a good fit, Google CoLab is a robust alternative.

["Google CoLab Instructions"](https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/google-colab-instructions.md), developed by Spring and Fall 2021 graduate teaching assistant [Subhadyuti Sahoo](https://github.com/SDSAHOO703).

See also:
- ["Welcome to Colaboratory"](https://colab.research.google.com/notebooks/intro.ipynb) notebook from Google CoLab
