```python
from numpy import genfromtxt
csv = genfromtxt('data/good_case/aas_total1.csv', delimiter=',', dtype=['int', 'float'], skip_header=1)
```

- delimiter: csv文件每一列的分隔符
- dtype: csv文件每一列的数据类型，只传一个类型时每一列都为该类型，传列表时，每一列为对应类型
- skip_header: 跳过前几行，默认为0，如果csv的第1行为表头则可以设置skip_header=1