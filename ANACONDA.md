# Anaconda 
> a distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.

[Windows](##anaconda-for-windows)
[Linux](##anaconda-for-linux)
## Anaconda for Windows 
---
### Installation

[Download the Anaconda Installer for Windows](https://docs.anaconda.com/anaconda/install/windows/)
** Check Add Anaconda3 to my PATH environment variable **

### Creating a Conda Environment
Open the Anaconda Prompt
```cmd
(base) C:\Users\temp>conda create --name <NAME> python=<VERSION>
(base) C:\Users\temp>conda activate <NAME>
```

### Adding Packages
Open the Anaconda Prompt and switch to desired conda environment
```cmd
(base) C:\Users\temp>conda activate <NAME>
(<NAME>) C:\Users\temp>conda install <PACKAGE>
(<NAME>) C:\Users\temp>pip install <PACKAGE>
```

### How Do I Know What Environment I am In?
It's the name within the parenthensis of the Anaconda Prompt. The default environment is called base.
```cmd
(base) C:\Users\temp>
```
You conda also list all the environments and see which one has a star (*) next to it.
```cmd
(base) C:\Users\temp>conda info --envs
# conda environments:
# 
base                * C:\Users\temp\anaconda3
nlp                   C:\Users\temp\anaconda3\envs\nlp

(base) C:\Users\temp>conda env list
# conda environments:
# 
base                * C:\Users\temp\anaconda3
nlp                   C:\Users\temp\anaconda3\envs\nlp

```

### How Do I Switch Environments?
To switch back to **base** you can use `deactivate` or `activate base`

### How Do I Export My Anaconda Environment?
You can export your environment into YAML format
> YAML is a recursive acronym meaing (YAML Ain't Markup Language)

To do this open Anaconda Prompt.
```cmd
(base) C:\Users\temp>conda env export --name <ENVNAME> > ENVNAME.yml
(base) C:\Users\temp>conda env export --name nlp > nlp.yml
```

## Anaconda for Linux
---
*TBD*