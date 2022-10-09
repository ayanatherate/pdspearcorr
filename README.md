
<h2> Python package for easy spearman's rank correlation coef comparison for continuous features in Pandas DataFrames (similar to data.corr() for default pearson's coef in Pandas) </h2> 

<h3>Run: </h3>

```
git clone https://github.com/ayanatherate/lyricscraper.git
cd pdspearcorr 
pip install -r requirements.txt
```

<br>
<h3>Open any Notebook/IDE: </h3>

```
import pandas as pd
from pdspearcorr import spearcorr
from sklearn import datasets

iris = datasets.load_iris()
iris_df=pd.DataFrame(iris.data)
iris_df.columns=['sepal_len', 'sepal_wid', 'petal_len', 'petal_wid']


spearcorr(data)
```
<img width="233" alt="image" src="https://user-images.githubusercontent.com/59755186/194780467-953738b6-760f-45dc-81f1-82b1fead00c7.png">

```
spearcorr(data)['sepal_len']

```
<img width="149" alt="image" src="https://user-images.githubusercontent.com/59755186/194780556-b233ce49-0788-4c54-bff7-739518ff94e0.png">
```
spearcorr(data,plot_htmp=True)

#Alternatively for plotting heatmap, can also use sns.heatmap(spearcorr(data))

```
<img width="477" alt="image" src="https://user-images.githubusercontent.com/59755186/194780600-295fd3d9-6bdb-4fe7-9511-d204747f097e.png">


