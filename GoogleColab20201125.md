# Jupyter Notebook
```
https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks
```
###  EDA (Exploratory Data Analysis)探索式資料分析
```
探索式資料分析是運用視覺化或基本統計等工具，來對資料有個初步的認識，以利後續對資料進行複雜或嚴謹的分析。

主要能幫助我們認識資料中三個部分：
1.瞭解資料，獲取資料的資訊、結構和特點。
2.檢查有無離群值或異常值，看資料是否有誤。
3.分析各變數間的關聯性，找出重要的變數。

進行EDA能檢查資料是否符合分析前的假設、在模型建立前先發現潛在的錯誤，並進一步調整分析方向。

https://ithelp.ithome.com.tw/articles/10213384
```
```
Exploratory data analysis in Python
https://nbviewer.jupyter.org/github/Tanu-N-Prabhu/Python/blob/master/Exploratory_data_Analysis.ipynb
```
###
```
from IPython.lib.display import YouTubeVideo
# An introduction to Python by Google.
#YouTubeVideo('tKTZoB2Vjuk') 
YouTubeVideo('jTp-tPrsdmE') 
```
###
```
from IPython.display import Image
Image(url='http://python.org/images/python-logo.gif')
```
###
```
from IPython.display import Math
Math(r'N(x) = \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x} e^{-
\frac{z^2}{2}}\, dz')
```
###
```
from IPython.display import HTML
table = """<table>
<tr>
<th>Header 1</th>
<th>Header 2</th>
</tr>
<tr>
<td>row 1, cell 1</td>
<td>row 1, cell 2</td>
</tr>
<tr>
<td>row 2, cell 1</td>
<td>row 2, cell 2</td>
</tr>
</table>"""
HTML(table)
```
