# `Lab 1b` Installation of the CHEME 4/5800 Toolchain (Anaconda, VSCode, Julia, GitHub, etc.)

## Overview
This lab will walk you through the CHEME 4/5800 toolchain installation. This toolchain includes the following software (all of which are free and open source):

* [Julia](https://julialang.org) - a high-level, high-performance, dynamic programming language that we'll use in the course (along with [Python](https://www.python.org) and other languages such as [C/C++]()) to demonstrate concepts in computational engineering.
* [GitHub Desktop](https://desktop.github.com) - a graphical user interface for the [Git](https://git-scm.com) version control system. We'll use GitHub Desktop to manage the code that we write in the course.
* [Visual Studio Code](https://code.visualstudio.com) - a code editor that supports various programming languages and file formats. We'll use VSCode to write and edit code in the course.
* [Anaconda](https://www.anaconda.com/products/individual) - a Python distribution that includes the [Jupyter Notebook](https://jupyter.org) and [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) interactive development notebook environments.

### Stretch goal
After installing these tools, our stretch goal is to test our installation by running a simple ["Hello World"](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) program written in Julia. However, if we don't finish today, we'll do it in the next lab.


## Installing Julia
This course uses the [Julia](https://julialang.org) programming language. You can find the installation instructions for Julia [here](https://julialang.org/downloads/). 
* On `Windows,` please check the `Add Julia to Path` checkbox during installation. This will allow you to run Julia from the command line.
* On `MacOS,` please follow the instructions to add Julia to your path found [here](https://julialang.org/downloads/platform/#macos). This will allow you to run Julia from the command line.

## Installing Anaconda
This course uses [Anaconda](https://www.anaconda.com/products/individual) as a Python distribution. You can find the installation instructions for Anaconda [here](https://docs.anaconda.com/anaconda/install/). If you still need a Python installation on your machine, we recommend installing [Anaconda](https://www.anaconda.com/products/individual).  

## Installing Visual Studio Code
This course uses [Visual Studio Code](https://code.visualstudio.com) as a code editor. You can find the installation instructions for Visual Studio Code [here](https://code.visualstudio.com/download). 
* Once you install Visual Studio Code, you must install the [Julia extension](https://www.julia-vscode.org) for Visual Studio Code. You can find the installation instructions for the Julia extension [here](https://www.julia-vscode.org/docs/stable/gettingstarted/).
* you'll also need to install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for Visual Studio Code. You can find the installation instructions for the Python extension [here](https://code.visualstudio.com/docs/languages/python).
* Once you have installed [Anaconda](https://www.anaconda.com/products/individual), you can install the [IJulia](https://github.com/JuliaLang/IJulia.jl) package, which will allow you to use [Jupyter](https://jupyter.org) with [Julia](https://julialang.org). To do this, open the `Julia REPL` (which you can open by typing `julia` in the terminal window in VSCode) and type the following commands:

```julia
using Pkg
Pkg.add("IJulia")
```

## Installing GitHub Desktop
This course uses [GitHub](https://github.com) to manage our code. You can find the installation instructions for GitHub Desktop [here](https://desktop.github.com). 
* Once you install the GitHub desktop, you can download the labs for the course by clicking on the `Code` button on the [lab GitHub repository](https://github.com/varnerlab/CHEME-4800-5800-Labs-AY-2024.git) and then clicking on the `Open with GitHub Desktop` button. This will open GitHub Desktop and allow you to download the labs for the course.
* Alternatively, you can copy the URL for the lab and paste it into the URL tab accessible from the `Add > Clone a repository` drop-down box in GitHub Desktop. This will allow you to download the labs into a local directory on your machine.

## Stretch goal: Testing your installation
Once you have installed the software listed above, you can test your installation by running the following commands in the `Julia REPL` (which you can open by typing `julia --project=.` command from the `week-1/Lab-1b` directory in the terminal window in VSCode):

```julia
include(joinpath("test", "runtests.jl"));
```
