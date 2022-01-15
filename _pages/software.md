---
layout: infolab-toplevel
title: Software
permalink: /software/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

## multinet (R)

<figure style="width:50%">
<img src="/assets/images/software/r_multinet.png"
         alt="The multinet library used inside RStudio" />
    <figcaption>The multinet library used inside RStudio.</figcaption>
</figure>

The <a href="https://cran.r-project.org/web/packages/multinet/index.html"> `R multinet` library</a> was first released on CRAN in 2017 and provides functions to analyse multilayer networks. To install it, you only need an Internet connection and a recent version of `R`. You can do that by typing:

    install.packages("multinet")
    
Here you can find <a href="https://github.com/uuinfolab/r_multinet">documentation and source code</a>, and register bugs or feature requests. 

## uunet.multinet (Python)

The  <a href="https://pypi.org/project/uunet/">`Python uunet.multinet`</a> library is a recent porting of the `R multinet` library, available on PyPI. To install it, you only need an Internet connection and a recent version of `Python` and `pip`. You can do that by typing:

    pip install uunet
    
Here you can find <a href="https://github.com/uuinfolab/py_multinet">documentation and source code</a>, and register bugs or feature requests. 

## uunet (C++)

The <a href="https://github.com/uuinfolab/uunet">`C++ uunet`</a> library contains most of the code behind the `R` and `Python` libraries for multilayer network analysis, in addition to other code for network and data analysis we develop at the Infolab. 

## Code for paper replicability

The code to replicate experiments in our papers is available from the <a href="../publications">Publications</a> page.
