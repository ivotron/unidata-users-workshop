# 2015 Unidata Users Workshop

[Complete information on the 2015 Unidata Users Workshop](http://www.unidata.ucar.edu/events/2015UsersWorkshop/)

## Python Instructions

A number of demonstrations will make use of the Jupyter Project (formerly
IPython Notebook) technology. For participants who wish to use Python during the
workshop, please follow the instructions below. To save time, we suggest
following these steps before your arrival at the workshop.

1. [Install Miniconda (Python 2.7) from Continuum Analytics](http://conda.pydata.org/miniconda.html). ([Determine if your OS 32 or 64 bit](http://www.akaipro.com/kb/article/1616#os_32_or_64_bit).)
2. Once Miniconda is installed, from the command line (e.g., OS X terminal, cmd.exe), run these instructions:

```
conda create -n workshop-scikit python=2 pip numpy scipy matplotlib pandas ipython-notebook netcdf4 scikit-learn scikit-image basemap
conda create -n workshop-xray python=2 pip numpy scipy matplotlib ipython-notebook pandas netcdf4 dask xray
conda create -n workshop-kevin python=2 pip numpy scipy matplotlib ipython-notebook netcdf4 basemap requests
conda create -n workshop-basic python=2 ipython-notebook
```

### metpy and siphon installation

```
conda create -n workshop-metpy python=2 pip numpy scipy matplotlib ipython-notebook netcdf4
```
#### on unix

```
source activate workshop-metpy && pip install metpy siphon
```

If this command causes an error see note below about bash.

#### on windows

```
activate workshop-metpy
pip install metpy siphon
```


### From a Unix command line (e.g., OS X terminal)
**If your default shell is NOT bash, first type `bash`.**
To activate or switch to a conda environment, you can `source activate
<environment>`. For example,

```
source activate workshop-xray
```

To switch and/or deactivate environments:

```
source deactivate
source activate <environment>
```


### From a Windows command line (e.g., cmd.exe)

To activate or switch to a conda environment, you can `activate
<environment>`. For example,

```
activate workshop-xray
```

To switch and/or deactivate environments:

```
deactivate
activate <environment>
```


### jupyter notebook

The presenters will probably ask you to run examples in the `ipython notebook`.
You may wish to create a folder on your desktop, and from the command line `cd`
to that folder, `activate` (see above) an environment, and start the notebook
with the `ipython notebook` command. Once this software is in place, Unidata
Users Workshop staff and presenters will instruct participants how to make use
of this software.

#### inline graphics

You will probably be doing matplotlib visualizations in which case you will want
to inline the graphics with this command:

```
%matplotlib inline
```

### 2015 Unidata Users Workshop Github Repository

Presenters, participants and staff are encouraged to make use of this github
repository for sharing of presentations and any material relevant to the Users
Workshop.

### Specific download for files used in Kevin Tyle's hands-on session:
http://www.atmos.albany.edu/facstaff/ktyle/triennial/
(Download the zip file; extract it; and then ideally cd into that directory and launch ipython notebook from there)

### When the workshop is over, how can I continue using these technologies?

#### git

We have been using git version control technology to share and collaborate on
the workshop material. The problem is git is not easy to use. Fortunately, there
are git clients/apps/user interfaces that can make git less painful. One such
tool is a tool called
[SourceTree](https://www.atlassian.com/software/sourcetree). If git seems
intimidating, please consider using a git client such as SourceTree to obtain
the workshop material or to interface with other git repositories.

#### conda

The other tool we have been using is conda. conda has made working with Python
scientific programming environment *much* easier. This README explains how to
download and install conda. Moreover, many, many scientific programming
libraries are distributed via conda. Hopefully, conda should satisfy most of
your needs for installing scientific computing libraries.

#### Unidata Training Workshops

Unidata will be providing git and conda training at the
[Using Unidata Technologies with Python](https://www.unidata.ucar.edu/events/2015TrainingWorkshop/#classes)
, July 20 - 22.


### Questions

If you have questions about these instructions, please contact
<mailto:support@unidata.ucar.edu>.
