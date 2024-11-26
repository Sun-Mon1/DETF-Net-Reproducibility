# DETF-Net Reproducibility Repository

This repository contains partial implementations and configurations for DETF-Net, a segmentation network designed for high-accuracy retinal vessel segmentation. The provided files aim to enhance reproducibility while safeguarding certain proprietary aspects of the research.

---

## **Repository Structure**
The repository includes partial core modules, data processing scripts, and configurations for various backbone models. Below is the directory overview:

### **1. `dataprocess/`**
- **`data_process.py`**: Script for preprocessing input data.
- **`process_label.py`**: Script for processing labels used in training.

### **2. `mycode/`**
Core modules implementing key functionality:
- **`EFF2d.py`**: Detail Feature Enhancement Function.
- **`DFF2d.py`**: Dynamic Feature Fusion function.
- **`MSAF2d.py`**: Multi-Scale Attention Fusion.
- **`SFFusion2d.py`**: Sub-feature fusion module.
- **`RefConv.py`**: Refinement convolutional block.

### **3. `configs/`**
Configuration files for integrating DETF-Net with multiple backbone architectures:
- **`deeplabv3/`**/**`knet/`**, **`maskformer/`**, **`mask2former/`**, **`swin/`**:
  - Partial configuration files to demonstrate compatibility with respective models.
---

## **Usage**

### **1. Data Preprocessing**
Use scripts in the `dataprocess/` folder to prepare input data and labels:
```bash
python dataprocess/data_process.py
python dataprocess/process_label.py
```

### **2. Model Integration**
Utilize the configuration files in the `configs/` folder to set up and run experiments with DETF-Net modules integrated into various backbone architectures.

### **3. Custom Modules**
Modules in `mycode/` demonstrate the core functionality of DETF-Net's DFEM and DTFM components. These can be integrated with other segmentation frameworks.

---

## **Example Configurations**
The `configs/` directory includes example setups for:
- DeepLabv3 with ResNet backbones.
- K-Net and Mask2Former adaptations.
- Swin Transformer backbone integration.

---

## **License**
This repository is shared under a research-only license. The provided code is intended for academic review and reproducibility purposes and is not licensed for commercial use.

---

## **Future Work**
We aim to further extend the repository by:
1. Including additional datasets for broader validation.
2. Providing inference scripts for easier evaluation of DETF-Net's performance.
3. Incorporating lightweight design adaptations to improve deployment on resource-constrained devices.
4. Uploading more complete versions of the implementation to further enhance reproducibility.

---

