# Environmental Sound Classification using ANN (UrbanSound8K)

This project classifies environmental sounds (e.g., dog bark, siren, engine) using a simple Artificial Neural Network (ANN) trained on MFCC features from the UrbanSound8K dataset.

## 🔧 Features
- 10-class classification using predefined UrbanSound8K folds
- ANN model with ReLU, Dropout, and Softmax output
- Input features: MFCC (120 × 173)
- Implements 10-fold cross-validation
- Written in PyTorch
- Can test various sounds by giving the path to the audio (must be within the class range)

## 📁 Dataset
- UrbanSound8K (not included in repo)
- Make sure to download and place it in the appropriate folder

## 📦 Dependencies
- Python 3.8+
- PyTorch
- NumPy
- Librosa
- scikit-learn
- Matplotlib

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/JigyasPritam/Environmental_Sound_Classification_IITG.git
   cd Environmental_Sound_Classification_IITG
2. Install Dependencies
     ```bash
    pip install -r requirements.txt

## 🧪 Evaluation

The model is evaluated using the official 10-fold cross-validation setup from the UrbanSound8K dataset.  
For each fold:
- The model is set to evaluation mode (`model.eval()`).
- Predictions are made on the test set using `torch.no_grad()` to disable gradient computation.
- Accuracy is calculated by comparing predicted and true labels.
- Fold-wise accuracy is stored and displayed.

After all 10 folds:
- The average accuracy is computed and reported across all folds.


## 📜 License

MIT License

## 🙏 Acknowledgments

- UrbanSound8K dataset by Justin Salamon et al.
- https://www.youtube.com/watch?v=mHPpCXqQd7Y
- https://www.researchgate.net/publication/372738035_A_Deep_Learning_Approach_for_Urban_Sound_Classification
- https://github.com/mariostrbac/environmental-sound-classification
