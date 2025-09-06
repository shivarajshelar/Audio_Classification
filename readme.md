# 🎵 Audio Classification with Deep Learning  

This project uses **UrbanSound8K** dataset and a **Convolutional Neural Network (CNN)** to classify different types of environmental sounds. It includes preprocessing (resampling, padding, and MFCC feature extraction), model training, and an interactive **Gradio app** for testing predictions.  

---

## 🚀 Features  
- Load and preprocess audio files using **Librosa**  
- Extract MFCCs and apply padding for consistent input  
- Train a **CNN model** with multiple Conv2D + Pooling layers  
- Evaluate accuracy and loss  
- Deploy using **Gradio UI** for real-time predictions  

---

## ⚙️ Installation  

```bash
# Create virtual environment
conda create  -p venv audio_dl  python==3.10 -y

# activate the conda
conda activate audio_dl/


# Install dependencies
pip install -r requirements.txt
```
```bash 
# all Important Library
TensorFlow / Keras -- Deep learning framework for CNN model

Librosa --Audio processing (resampling, MFCC extraction)

NumPy -- Numerical computations

Pandas -- Data handling (UrbanSound8K metadata CSV)

Scikit-learn -- StandardScaler for feature normalization

Gradio -- Web UI for testing the model interactively

Matplotlib/ seaborn / -- For plotting results/visualizations

```
---

## 🧠 Model Architecture  
- 4 × Conv2D + BatchNorm + MaxPooling layers  
- Dense layer (64 units, ReLU)  
- Dropout (0.3) for regularization  
- Softmax output for classification  

---

## 🎤 Usage  

### Train the Model  
Open `trial.ipynb` in **VS Code / Jupyter** and run the cells.  

### Launch Gradio App  
After training:  
```bash
 from `trial.ipynb` notebook last cell
```
Then open the provided `localhost` link to test your audio files.  

---

## 📊 Dataset  
👉 [UrbanSound8K Dataset on Kaggle](https://www.kaggle.com/datasets/chrisfilo/urbansound8k)
- **UrbanSound8K** dataset: 8,732 labeled sound excerpts (≤ 4s)  
- Classes include: air_conditioner, car_horn, children_playing, dog_bark, drilling, engine_idling, gun_shot, jackhammer, siren, and street_music.  

---

## ✨ Demo  
Upload or record an audio clip → get **Predicted Class** instantly.  
"# Audio_Classification" 
"# Audio_Classification" 
"# Audio_Classification" 
