![logo](logo.png)


# General Engine for Eco-Evolutionary Simulations

This is the repository for the R-package of the Gen3sis engine.

Gen3sis is a spatially-explicit eco-evolutionary mechanistic model with a modular implementation. It allows exploring the consequences of ecological and macroevolutionary processes across realistic or theoretical spatio-temporal landscapes.

Gen3sis is licensed under a [GPLv3 License](https://www.gnu.org/licenses/gpl-3.0.html) ETHZ 2020 <doi.org/10.5905/ethz-1007-251>

Package authorship according to: http://epub.wu.ac.at/3269/1/Report114.pdf

### How to install gen3sis

Gen3sis is on CRAN. So, to install the latest CRAN release, just run in R

```{r}
install.packages("gen3sis")
```

### How to run one simple simulation

Load and run a simulation with the desired config and landscapes. Exemple data is provided with the package
```{r}
library("gen3sis")
sim <- run_simulation(config = "config_xD.R", input_directory = "./simulations/World")

```
A summary statistics is stored at 'sim' more data can be save using the oberver function

### How to visualize a simulation

Plot the summary statistics of a simulation

```{r}
plot_summary(sim)
```

### Check package version

Make sure you have the latest gen3sis version

```{r}
#print package version
paste("GEN3SIS version:", packageVersion("gen3sis"))
```
