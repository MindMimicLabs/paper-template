Below can be found the necessary steps to re-generate the paper from the raw `.rmd`s.
If re-generation of the results is also desired, please refer to the instruction in the [code readme](../code/README.md).
All the results, tables, and figures should be stored in the `./results` folder so the regeneration of the paper should be very fast.

# Steps

1. Double click on `index.rmd file`
2. Click knit

# Packages

The paper itself needs `bookdown` and `kableExtra` in addtion to the packages used in the analysis.
Install them as below.

```{r}
install.packages('rmarkdown')
install.packages('kableExtra')
install.packages('bookdown')
install.packages('tinytex')

tinytex::install_tinytex()
```