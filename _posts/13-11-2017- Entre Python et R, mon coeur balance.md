
```python

### Représenter graphiquement nos données
#### Histogramme
from matplotlib import pyplot
from pandas import read_csv
nom_fichier = 'pima-indians-diabetes.data.csv'noms_variables = ['preg','plas','pres','skin','test','mass','pedi','age', 'class']
donnees  = read_csv(nom_fichier, names = noms_variables)
donnees.hist()
pyplot.show() ```


![png](output_0_0.png)

```python ### Représenter graphiquement nos données
#### Densité de probabilité
from matplotlib import pyplot
from pandas import read_csv
nom_fichier = 'pima-indians-diabetes.data.csv'
noms_variables = ['preg','plas','pres','skin','test','mass','pedi','age', 'class']
donnees  = read_csv(nom_fichier, names = noms_variables)
donnees.plot(kind = 'density', subplots = True, layout = (3,3), sharex = True)
pyplot.show() ```
![png](output_1_0.png)

```python
# Box and Whisker Plotsfrom matplotlib 
import pyplotfrom pandas 
import read_csvfilename = "pima-indians-diabetes.data.csv"
names = ['preg', 'plas', 'pres', 'skin', 'test', 'mass', 'pedi', 'age', 'class']
data = read_csv(filename, names=names)
data.plot(kind='box', subplots=True, layout=(3,3), sharex=False, sharey=False)
pyplot.show() ```
![png](output_2_0.png)


