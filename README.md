# Group 07 - UCI EMG Physical Action Classification (CSE475)

## 1. Overview
- **Group:** Group 07
- **Dataset:** UCI EMG Physical Action Data Set ([Dataset ID 213](https://archive.ics.uci.edu/dataset/213/emg+physical+action+data+set))
- **Dataset Slug:** `EMG_Action`
- **Track:** Time-Series Signal Processing & Action Recognition

## 2. Dataset Specifications
- **Sensors:** 8-channel surface electromyography (sEMG) collected via Delsys wireless apparatus.
- **Muscle Channels:** Right Bicep (ch1), Right Tricep (ch2), Left Bicep (ch3), Left Tricep (ch4), Right Thigh (ch5), Right Hamstring (ch6), Left Thigh (ch7), Left Hamstring (ch8).
- **Subjects:** 4 participants (3 Male, 1 Female aged 25–30).
- **Classes (20 Total):**
  - **10 Normal Actions:** Bowing, Clapping, Handshaking, Hugging, Jumping, Running, Seating, Standing, Walking, Waving.
  - **10 Aggressive Actions:** Elbowing, Frontkicking, Hammering, Headering, Kneeing, Pulling, Punching, Pushing, Sidekicking, Slapping.

## 3. Results Summary

| Model | Cross-Validation | Accuracy | Macro F1-Score | Key Components |
| :--- | :---: | :---: | :---: | :--- |
| Random Forest (Handcrafted Features) | 5-Fold CV | -- | -- | MAV, RMS, Wavelet features |
| 1D-CNN Baseline | 5-Fold CV | -- | -- | Standard 1D convolutions |
| **Proposed Model (1D-CNN + BiLSTM + Attention)** | **5-Fold CV** | **--** | **--** | **Spatial-Temporal Attention** |

## 4. How to Run

1. **Install Dependencies:**
   ```bash
   pip install ucimlrepo torch numpy pandas scikit-learn matplotlib seaborn
