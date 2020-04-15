Below can be found a list of data manulipation scripts that help make this work posible.

# Packages/Modules

Describe 

All scripts have been tested on Python 3.8.2.
The below modules are need to run the scripts.
The scripts were tested on the noted versions, so YMMV.
**Note**: not all modules are required for all scripts.
If this it the first time running the scripts, the modules will need to be installed.
They can be installed by navigating to the `~/code` folder, then using the below code.

* nltk 3.4.5
* progressbar2 3.47.0

```{shell}
pip install -r requirments.txt
python -c "import nltk;nltk.download('punkt')"
```

All scripts have been tested on R/R Studio 3.6.2/1.2.5019.
The below packages are need to run the scripts.
The scripts were tested on the noted versions, so YMMV.
**Note**: not all packages are required for all scripts.
If this it the first time running the scripts, the packages will need to be installed.
They can be installed using the below code then re-starting RStudio.

* readr 1.3.1
* rlist 0.4.6.1
* dplyr 0.8.3
* jsonlite 1.6
* magrittr 1.5
* pROC 1.16.1
* stringr 1.4.0
* tidyr 1.0.0
* tidyverse 1.3.0
* lubridate 1.7.4

```{r}
install.packages(c('readr', 'rlist', 'dplyr', 'jsonlite', 'pROC', 'stringr', 'tidyr', 'tidyverse', 'lubridate', 'magrittr'))
```

# Scripts

1. [Combine and clean the data](./CombineAndCleanData.rmd) to get rid of all the data that is not necessary for the analysis.
   This will create the clean file `~/data/clean_loan_data/loans.csv`.
2. [Generate the sampled datasets](./GenerateSampledDatasets.rmd) to assess the effect of an unbalanced analysis.
   This will create several datasets in the folder `~/data/sampled_data_datasets`
3. [Run the Fuzzy](./RI_fuzzy.rmd) RI algorithm on a given folder.
   This will create the results file `~/results/RI_fuzzy.{folder}.RData`.
4. [Run the Parcelling](./RI_parcelling.rmd) RI algorithm on a given folder.
   This will create the results file `~/results/RI_parcelling.{folder}.RData`.
5. [Run the Simple Augmentation](./RI_simple_augmentation.rmd) RI algorithm on a given folder.
   This will create the results file `~/results/RI_simple_augmentation.{folder}.RData`.
6. [Generate the Monte-Carlo grid](./GenerateMonteCarloGrid.rmd) to establishing the grid search parameters.
   This will create the configuration file `~/data/simulated/grid.json`.
