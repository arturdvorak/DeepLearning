# Deep Learning with Pima Indians Diabetes Dataset

This project contains a deep learning model to classify diabetes outcomes using PyTorch and PyTorch Lightning.

- Dataset: `pima-indians-diabetes.data.csv`
- Notebook: `Deep Learning.ipynb`

---

## Project Structure

### Part 1: EDA and Data Processing  
- Exploratory analysis of the dataset  
- Handling missing values, scaling, and feature overview  

### Part 2: Data Processing Summary and Pipeline  
- Overview of preprocessing steps  
- Final data pipeline for model training  

### Part 3: Classification with PyTorch  
- **3.1** Neural Network Model (1 hidden layer with 16 units, ReLU)  
- **3.2** Neural Network Models: Various Architectures  
- **3.3** Neural Network Models: Architecture Comparison  
- **3.4** Optimizer Tuning for Best Architecture ([256, 128, 64, 32, 16], ReLU)  
- **3.5** Optimizer Comparison for Best Architecture  
- **3.6** PyTorch Lightning Implementation for Best Architecture ([256, 128, 64, 32, 16], ReLU, SGD)  
- **3.7** Manual PyTorch vs PyTorch Lightning Comparison  

### Part 4: Convolution Operations  
- **4.1** 1D Convolution: Custom implementation without deep learning libraries  
- **4.2** 2D Convolution: Custom implementation on real images  
- **4.3** Edge Detection with Sobel Operator  

### Part 5: Conclusions  
- Summary of performance and model selection  
- Convolution insights and image processing observations