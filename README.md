# matplotlib-abaqus-v6.14-1
Allow abaqus(v6.14-1) to use matplotlib in its build-in python scripts environment.

The advantage to let abaqus python use matplotlib module is you can use python to read your abaqus odb file and operate the result data like stress and strain, and the plot it out and save as pdf or eps file that can used in latex.

## python modules
This project include the following python modules. ONLY tested on `abaqus 6.14-1`.
* matplotlib (1.3.1)
* dateutil (2.4.1)
* six (1.9.0)
* pyparsing (2.0.3)

## how it works
Copy the python modules to the abaqus python package folder:
```
...\SIMULIA\Abaqus\6.14-1\tools\SMApy\python2.7\Lib\site-packages
```

## test
* Run the python script `matplotlib_test.py` in abaqus CAE. if abaqus build-in python can include the matplotlib module successfully, there will be a plot window pop out.

* run the python script`test_link_mpl_toolkits.py` in abaqus CAE, to test if the abaqus python can import `mpl_toolkits` module.
