# TTim, A Multi-Layer, Transient, Analytic Element Model

## Introduction

TTim is a computer program for the modeling of transient multi-layer flow with analytic elements
and consists of a library of Python scripts and FORTRAN extensions.
TTim is based on the Laplace-transform analytic element method. The solution is computed analytically
in the Laplace domain and converted back to the time domain numerically usig the algorithm of De Hoog, Stokes, and Knight.
TTim may be applied to an arbitrary number of aquifers and leaky layers.
The head, flow, and leakage between aquifers may be computed semi-analytically at any point in space and time.
The design of TTim is object-oriented and has been kept simple and flexible.
New analytic elements may be added to the code without making any changes in the existing part of the code.
TTim is coded in Python; use is made of FORTRAN extensions to improve performance.

## TTim Changes

### Version 0.3
In version 0.3, the numbering of the layers in TTim has changed. Layers are numbered from the top down starting at number 0.
(in TTim versions prior to 0.3, layer numbers started at 1).

## Installation

**Python versions:**

TTim requires **Python** 2.7 and can be installed from PyPI.
The PyPI installation includes compiled versions of the FORTRAN extension
for both Windows and MaxOS.


**Dependencies:**

TTim requires **NumPy** 1.9 (or higher) and **matplotlib** 1.4 (or higher). T

**For base Python distributions:**

To install TTim, open a command prompt and type:

    pip install ttim

To update TTim type:

    pip install ttim --upgrade

To uninstall TTim type:

    pip uninstall ttim
    
**Testing installation:**

    ipython
    import ttim.ttimtest
    
An example model is imported and two graphs are shown. When this is run from the regular Python prompt (not IPython), the
model is created and solved but the figure is probably not shown (depending on your default settings of matplotlib). 


## Documentation

* The manual is available from the docs directory or can be viewed [here](https://github.com/mbakker7/ttim/blob/master/docs/timml.pdf).
Once you click on this link, you can click on the [Raw] button to download the pdf file. 
* Example Notebooks are available from the git repository.
