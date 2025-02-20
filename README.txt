# Readme file for the Bayes-light-scattering codes
# Please do not forget to set up the path as the local path of this folder before running the following scripts
# Feel free to contact Fan Yin via email, yinf2@uci.edu, if you have any questions.

#####
# prerequisites
These scripts require R (https://cran.r-project.org/) to run as well as the following packages (and any dependencies): `AICcmodavg`, `boot`, `coda`, `doParallel`, `dplyr`, `foreach`, ``ggmcmc`, `ggplot2`, `ggpubr`, `invgamma`, `mcclust`, `mclust`, `MCMCvis`, `parallel`, `R2jags`, `R2WinBUGS`, `rjags`, `robustbase`, `scales`, `sna`, `trunctnorm`, and `xtable`.  These can be installed from within R using the `install.packages()` command.  Note that JAGS is also needed; information on installing JAGS can be found at https://mcmc-jags.sourceforge.io/.


##### 
# simulation study 
source("./simulation/lysozyme.simulation.study.lognormal.R")
source("./simulation/lysozyme.simulation.study.noadjustment.R")

# summarize the results of simulation study
source("./simulation/lysozyme.simulation.summary.R")


#####
# case study: lysozyme
source("./lysozyme/lysozyme.main.R")


#####
# case study: gamma S crystallin
source("./gsc/gsc.main.R")


