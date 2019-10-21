# SSDD
## Severstal: Steel Defect Detection

This [competition](https://www.kaggle.com/c/severstal-steel-defect-detection)

### The dataset:

To install and config this command line api first, check [here](https://github.com/Kaggle/kaggle-api)
```
mkdir ssdd/;
cd ssdd;
kaggle competitions download severstal-steel-defect-detection
```

### References:
* [Helpful public kernels](doc/kernels.md)
* [UNet Paper](https://arxiv.org/pdf/1505.04597.pdf)

### Extra Package
* Package: [segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch)
```
pip install git+https://github.com/qubvel/segmentation_models.pytorch
```

### Save to JIT model
* ```jitcp --src="/home/paperspace/bestmodel_27.pth" --dst="jit_fpn_b6.pth" --model="fpn" --encoder="efficientnet-b6"```
* The [process notebook and doc](jitcp.ipynb)