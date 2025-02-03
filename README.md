# ICC for MRI analysis

- Have a look at the Literature folder for deeper understanding

## Data preparation

# SPM or first level analysis

- you can use beta or con images as input which measn you can use the beta images of the general linear model or contrast images betwen two or more regressor as input
- In this case one beta value contains all learning stages (1,2,3,4) and therefore shows the beta values for all task onsets calculated by the model 
- If you have a general linear model in which each beta value is a learning stage you have to adapt the script and load all beta images for sham in one list and stim in the other list

- if you like to have an ICC of the contrast task > control, use con images

### Software installed on the system

- python
- mamba or conda (virtual environemnt manager) (mamba is recommended)

-your terminal should change from 

```bash
$
```

to 

```bash
(base)$
```

- if you install conda change commands below to conda instead of mamba
- code ist written on Linux system so be careful and check the path strings you might have to change them

### main python package pyremli

-  [pyremli](https://pyrelimri.readthedocs.io/en/latest/)

### install packages via virtual environment

- create a conda virtual environment from the ICC.yml file (ask chatGDP or deepseek how to do that)
- or open the ICC.yml file with a text editor and install packages with "conda install" or "pip install"
- activate ICC environment like this

```bash
(base)$mamba env create -f environment.yml
(base)$mamba activate ICC
```

- your terminal should no show ICC instead of base

```bash
(ICC)$
```

### run script

- open a terminal an change directory to script path

```bash
ICC$ cd .../Example_Code_ICC
```

- open "juypter notebook" in terminal

```bash
ICC$ jupyter notebook
```

- open the "ICC_Ecample_code.ipynb" file in the editor
- run the script 

