## Project for INFO 550 FALL 2020

For this project, I try to evaluate the performance of Wald test in testing whether an addition biomarker will increase the accuracy of predicting a binary outcome.

The data used will be generated using Monte Carlo simualtions from a logistic regression, where values of biomarkers are independently normally distributed with common mean and variance.

There is no addition package require to perform the statistical analysis, but some packages will be needed to generate tables and plots. The required packages can be installed using `R` commands.

``` r
installed_pkgs <- row.names(installed.packages())
pkgs <- c("MASS", "knitr", "arsenal")
for(p in pkgs){
	if(!(p %in% install_pkgs)){
		install.packages(p)
	}
}
```


## Execute the analysis

To execute the analysis, from the project folder you can run 

``` bash
Rscript -e "rmarkdown::render('report.Rmd')"
```

This will create a file called `report.html` output in your directory that contains the results.