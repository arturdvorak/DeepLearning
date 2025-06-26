# Deep Learning with Pima Indians Diabetes Dataset

This project contains a deep learning model to classify diabetes outcomes using PyTorch and PyTorch Lightning.

- Dataset: `pima-indians-diabetes.data.csv`
- Notebook: `Deep Learning.ipynb`

---

## Project Structure

### Part 1: EDA and Data Processing  
- Exploratory data analysis  
- Feature inspection  
- Handling missing values and outliers  

### Part 2: Data Processing Summary and Pipeline  
- Normalization and transformations  
- Final preprocessing pipeline for model training  

### Part 3: Classification with PyTorch  

- **3.1 Neural Network Model (1 hidden layer with 16 units, ReLU)**  
  A baseline fully connected neural network was built using PyTorch. It uses one hidden layer with 16 units and ReLU activation. This model serves as a starting point for deeper architectural exploration.

- **3.2 Neural Network Models: Various Architectures**  
  Deeper models were tested using multiple hidden layers and different numbers of neurons to evaluate performance improvements. All models use ReLU activation and binary cross-entropy loss.

- **3.3 Neural Network Models: Various Architectures Comparison**  
  Architectures were compared using the **F1 score**, a balanced metric for imbalanced datasets. This helped identify the structure that best distinguishes between diabetic and non-diabetic outcomes.

- **3.4 Optimizer Tuning for Best Architecture ([256, 128, 64, 32, 16], ReLU)**  
  The best-performing architecture from 3.3 was selected and trained using different optimizers (SGD, Adam, RMSprop). Learning rates were tuned to maximize the F1 score and minimize loss.

- **3.4 Optimizer Comparison for Best Architecture ([256, 128, 64, 32, 16], ReLU)**  
  Different optimizers were compared based on their impact on F1 score and training stability. The comparison guided the selection of the final optimizer setup.

- **3.5 PyTorch Lightning for Best Architecture ([256, 128, 64, 32, 16], ReLU, SGD)**  
  The best architecture and optimizer setup was re-implemented using PyTorch Lightning for modular, efficient training.

- **3.5 PyTorch Manual and Lightning Comparison for Best Architecture ([256, 128, 64, 32, 16], ReLU, SGD)**  
  Manual PyTorch and Lightning implementations were compared side-by-side using F1 scores and training dynamics to ensure consistency.

- **3.6 1D Convolution**  
  A custom 1D convolution function was implemented from scratch without using PyTorch or TensorFlow. It was used to denoise synthetic signals and demonstrate the basics of convolution.

- **3.7 2D Convolution**  
  A custom 2D convolution operation was implemented and applied to RGB image arrays for feature detection.

- **3.8 Conclusions: 2D Convolution and Edge Detection**  
  The Sobel operator and other filters were applied to grayscale images. Their effectiveness for edge detection was evaluated and summarized.