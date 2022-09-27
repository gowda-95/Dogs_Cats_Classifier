# Classify Dog vs Cats

Train a custom CNN network for classification task and compare it's accuracy with that of ResNet-18 by using transfer learning.


## Requirements
Python version > = 3.6

PyTorch, Torchvision, matplotlib, NumPy, Pandas, PIL.

## Data

The [CATS_DOGS.zip](https://drive.google.com/file/d/1fuFurVV8rcrVTAFPjhQvzGLNdnTi1jWZ/view) is about 774Mb compressed, it should be downloaded and placed in [data folder](https://github.com/gowda-95/Dogs_Cats_Classifier/tree/main/data).

There are a total of 24994 images of various sizes. They are split into train and test folders as follows.

#### Image files directory tree
<pre>.
└── Data
    └── CATS_DOGS
        ├── test
        │   ├── CAT
        │   │   ├── 9374.jpg
        │   │   ├── 9375.jpg
        │   │   └── ... (3,126 files)
        │   └── DOG
        │       ├── 9374.jpg
        │       ├── 9375.jpg
        │       └── ... (3,125 files)       
        │           
        └── train
            ├── CAT
            │   ├── 0.jpg
            │   ├── 1.jpg
            │   └── ... (9,371 files)
            └── DOG
                ├── 0.jpg
                ├── 1.jpg
                └── ... (9,372 files)</pre>


## Results
|  | Custom network | ResNet-18 (finetuned) | ResNet-18 (frozen convnet) |
|---|--------|------------|---------------|
|Accuracy (50 epochs)| 82.43% | 96.16% | 97.63%|
