# Juliet-NDSS18-BinaryCodeSummary
The pre-processed Juliet, NDSS18 datasets for assembly code summarization (asm -> text). Dataset files can be found at the release page. Example data loading code:

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

