# [R package called PIPE](https://github.com/hfang-bristol/PIPE)

## @ Overview

> The [PIPE](http://www.genetictargets.com/PIPE) is a pleiotropy-driven framework for therapeutic target prediction and validation, with its validity illustrated using two systems of disorders as exemplars, generating `pleiotropy target index (PTI)` for neuropsychiatric disorders ([PTI-npd](http://www.genetictargets.pro/PIPE/portal/npd)) and inflammatory disorders ([PTI-ind](http://www.genetictargets.pro/PIPE/portal/ind)), respectively.

> Showcases, describing step-by-step instructions on how to use, are made reproducible for [neuropsychiatric disorders](http://www.genetictargets.pro/PIPE/showcase/npd) and [inflammatory disorders](http://www.genetictargets.pro/PIPE/showcase/ind).


## @ Installation


### 1. Install R

Please install R (version 4.2.1 or above); see https://cran.r-project.org

If installed on `Ubuntu`, please do so below assuming you have a `ROOT (sudo)` privilege.

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

# first, install basic packages: remotes, tidyverse, pbapply, ComplexHeatmap
BiocManager::install(c('remotes','tidyverse','pbapply','ComplexHeatmap'), dependencies=T)

# then, install the package 'PIPE' (now hosted at github)
BiocManager::install("hfang-bristol/PIPE", dependencies=T, force=T)

# check the package 'PIPE' successfully installed
library(PIPE)
```

## @ Contact

> Please drop [email](mailto:fh12355@rjh.com.cn) for bug reports or enquiries.


