# Repo Template

Describe the purpose of the project.
What result does it demonstrate?
What tools/techniques does it use?

# Tabula Rasa

The below steps can be taken to "re-play" the project's process.
Each step may refer to a different README.
In these cases, the step in that README will aslo be noted.
It is recomended you read the full README as sometimes a step may contain a shortcut or other prior assumed knoledge.

When the work is still _in-progress_ a note of TODO, DOING, DONE should be added to the front

01. Get the raw data.
    [Data instructions](./data/README.md)(step 1...N).
02. Describe some steps that need to be run
    [Code instructions](./code/README.md)(script 1...M).
03. Describe more steps that need to be run
    [Code instructions](./code/README.md)(script M+1...N).
04. Knit the paper.
    [Paper instructions](./paper/README.md)(script 1-2).


# Prerequisites

The following packages need to be installed.
You can use any method to install the prerequsits.
I recommend using [Chocolatey](https://chocolatey.org/install).
If you descide to use Chocolatey, open an _admin_ PowerShell prompt and run the code snipet below.

* [Python](https://www.python.org/downloads/)
* [R](https://cran.r-project.org/bin/windows/base/) + [R Studio](https://www.rstudio.com/products/rstudio/download/)
* 
  
```{ps1}
if('Unrestricted' -ne (Get-ExecutionPolicy)) { Set-ExecutionPolicy Bypass -Scope Process -Force }
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
refreshenv
choco install python3 -y
refreshenv
choco install r.project -y
refreshenv
choco install r.studio -y
```
