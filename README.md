# Juliet-NDSS18-BinaryCodeSum
The pre-processed Juliet, NDSS18 datasets for Assembly code summarization. Example data loading code:

```python

#LOADING Training Data CACHE

import gzip
import pickle
# cache = 'mne-desp.pkl'
cache = 'mne-opr-desp.pkl' # with oprands.

with gzip.open(cache, 'rb') as rf:
    ds = pickle.load(rf)
train_asm, test_asm, train_des, test_des = ds



```

