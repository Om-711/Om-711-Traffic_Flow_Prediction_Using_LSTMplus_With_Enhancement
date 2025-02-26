# Traffic Flow Prediction using LSTM with Feature Enhancement

## Overview
This repository contains the implementation of an improved LSTM-based model for short-term traffic flow prediction. The model leverages feature enhancement techniques, including noise smoothing and attention mechanisms, to improve prediction accuracy. The primary goal is to enhance the long-term memory of LSTM and make predictions more reliable in the presence of noisy data.

## Features
- **LSTM with Feature Enhancement**: Improved LSTM architecture incorporating additional features for better accuracy.
- **Noise Processing**: Data preprocessing techniques to remove anomalies and improve data quality.
- **Attention Mechanism**: Capturing high-impact traffic flow values to improve long-term dependencies.
- **Dataset**: Uses the PEMS dataset for real-world traffic flow prediction.

## Installation
To set up the environment, install the required dependencies:
```sh
pip install torch numpy pandas matplotlib shap lime scikit-learn
```

## Usage
### Training the Model
Run the training script to train the LSTM model:
```sh
python train_lstm.py
```

### Running XAI Methods
To analyze model interpretability using SHAP and LIME:
```sh
python explain_lstm.py
```

## Dataset
The model is trained and evaluated on the **PEMS08 dataset**, which contains traffic flow data collected from various locations. The dataset includes:
- **Traffic Flow (Volume)**
- **Occupancy**
- **Speed**

## Results
The model demonstrates superior performance in short-term traffic prediction by reducing error metrics:
- **Mean Absolute Error (MAE):** Lower compared to baseline LSTM models.
- **Mean Relative Error (MRE):** Improved accuracy through feature enhancement.
- **Root Mean Squared Error (RMSE):** Reduced due to better data preprocessing.

## Citation
If you use this repository in your research, please cite:
```
@article{yang2019traffic,
  title={Traffic flow prediction using LSTM with feature enhancement},
  author={Yang, Bailin and Sun, Shulin and Li, Jianyuan and Lin, Xianxuan and Tian, Yan},
  journal={Neurocomputing},
  volume={332},
  pages={320--327},
  year={2019},
  publisher={Elsevier}
}
```

