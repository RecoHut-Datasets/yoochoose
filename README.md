
This is the processed version of [v2](https://github.com/RecoHut-Datasets/yoochoose/tree/v2). 

Code used for processing:
```python
!pip install recohut==0.0.9-post1
from recohut.datasets.yoochoose import YoochooseDataset
ds = YoochooseDataset(root='/content/data', min_session_length=20, min_item_support=20)
```

Snapshot:
```
uid,timestamp,sid
87,1396851548.914,214652220
87,1396851560.979,214840483
87,1396851568.762,214840483
87,1396851961.516,214717286
87,1396851975.176,214558807
87,1396851992.159,214821300
87,1396852010.136,214826908
87,1396852019.987,214826908
87,1396852028.677,214826908
```

File sizes:
```
/content/data
├── [ 66M]  processed
│   ├── [ 66M]  yoochoose_train.txt
│   └── [263K]  yoochoose_valid.txt
└── [1.4G]  raw
    └── [1.4G]  rsc15-clicks.dat

 1.4G used in 2 directories, 3 files
```

Time Taken : 8 mins.