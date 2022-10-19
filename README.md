# [An R package `PIPE`](https://github.com/23verse/PIPE)

## @ Overview

> The [PIPE](http://www.genetictargets.pro/PIPE) is a pleiotropy-driven framework for therapeutic target prediction and validation, with its validity illustrated using two systems of disorders as exemplars, generating `pleiotropy target resources` for [`neuropsychiatric disorders`](http://www.genetictargets.pro/PIPE/portal/npd) and [`inflammatory disorders`](http://www.genetictargets.pro/PIPE/portal/ind), respectively. Also made available are [`functional modules`](http://www.genetictargets.pro/PIPE/portal/mod) and [`prioritisation map`](http://www.genetictargets.pro/PIPE/portal/map).


## @ Installation

### 1. Install R

Please install R (version 4.2.1 or above); see https://cran.r-project.org

If installed on `Ubuntu` (assuming you have a `ROOT (sudo)` privilege), please do so below

```ruby
sudo su
# here enter your password

wget http://www.stats.bris.ac.uk/R/src/base/R-4/R-4.2.1.tar.gz
tar xvfz R-4.2.1.tar.gz
cd ~/R-4.2.1
./configure
make
make check
make install
R # start R
```

### 2. Install R packages

```ruby
R # start R

# if the package 'BiocManager' not installed, please do so
if(!("BiocManager" %in% rownames(installed.packages()))) install.packages("BiocManager")

# first, install basic packages: remotes, tidyverse
BiocManager::install(c('remotes','tidyverse'), dependencies=T)

# then, install the package 'PIPE' (now hosted at github)
BiocManager::install("23verse/PIPE", dependencies=T, force=T)

# check the package 'PIPE' successfully installed
library(PIPE)
```


## @ Showcases

> Showcases, describing step-by-step instructions, are made reproducible for [`neuropsychiatric disorders`](http://www.genetictargets.pro/PIPE/showcase/npd), [`inflammatory disorders`](http://www.genetictargets.pro/PIPE/showcase/ind), [`functional modules`](http://www.genetictargets.pro/PIPE/showcase/mod), and [`prioritisation map`](http://www.genetictargets.pro/PIPE/showcase/map).


## @ Contact

> Please drop [email](mailto:fh12355@rjh.com.cn) for bug reports or enquiries.


