# pytorch-week4

Repository for my implementation of **"Learn PyTorch for Deep Learning in a Day"** by Daniel Bourke.

I watched the full ~26-hour YouTube tutorial and actively **typed and ran all code** in Google Colab, documenting each section below.

##  Video Outline & My Implementation

### 00 ‑ PyTorch & Deep Learning Fundamentals
- Introduced `torch` and tensors: creation, shape, datatype, device (CPU/GPU).
- Demonstrated basic tensor math, indexing/slicing, broadcasting.
- Explored interoperability: converting between NumPy arrays and PyTorch tensors.
- Applied `requires_grad`, gradient tracking, and manual backward passes.
- Learned seed setting and gradient accumulation nuances.  

### 01 ‑ PyTorch Workflow
- Covered dataset flow: `Dataset` → `DataLoader`.
- Loaded built-in datasets (e.g., MNIST/CIFAR10).
- Demonstrated batching, shuffling, multi-worker loading.
- Explored automatic differentiation via `autograd`.
- Built a full training loop with loss (`nn.CrossEntropyLoss`) and optimizer (`SGD`, `Adam`).
- Evaluated model and tracked metrics (accuracy/loss).  

### 02 ‑ Neural Network Classification
- Defined models using `nn.Module`, including `forward()` method.
- Explored `nn.Sequential` and common layers (Flatten, Linear, ReLU, Softmax).
- Trained classifier on a dataset (e.g., FashionMNIST/CIFAR10).
- Visualized performance across training epochs.  

### 03 ‑ Computer Vision
- Loaded image datasets from folders.
- Utilized data transforms (`transforms.ToTensor()`, normalization, augmentation).
- Defined CNN architectures: Conv2d, pooling, activations, flattening.
- Built custom training and validation loops for CNN.
- Visualized sample predictions and loss/accuracy curves.  

### 04 ‑ Custom Datasets
- Created a subclass of `torch.utils.data.Dataset` for loading custom images and labels.
- Implemented `__init__`, `__getitem__`, `__len__`.
- Used above with `DataLoader` to train the FoodVision‑Mini image classifier.
- Managed common data-loading issues (e.g., PIL image handling, worker threads).  

