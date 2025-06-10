# DeepFake_Detection_For_Media_Verification_Using_ResNext_LSTM
This project is a robust deepfake detection system built using Convolutional Neural Networks (ResNeXt) and Long Short-Term Memory (LSTM) networks. It processes video data to detect manipulated (fake) content by analyzing both spatial and temporal features. The solution includes a web-based interface for uploading videos and visualizing predictions through heatmaps.
## 🎥 Demo

👉 (https://drive.google.com/file/d/1SA7z437gHj5BF7-Uv2zM1OdGAODDJ53K/view?usp=sharing)  

## 🌟 Features

- 🔍 **Face Detection**: Uses OpenCV DNN to extract faces from video frames.
- 🧠 **ResNeXt + LSTM**: Captures both spatial (image-level) and temporal (sequence-level) features.
- 📊 **Heatmap Visualization**: Highlights suspicious regions in video frames.
- 🌐 **Web Interface**: Upload videos and view results interactively.
- ⚙️ **API Integration**: FastAPI backend connected to a Next.js frontend.
- 🛡️ **Firebase + Kinde Auth**: Secure login and user video submission.
- ☁️ **Colab Training**: Easily train and test the model in Google Colab.

## 🧠 Architecture
Video → Frame Extraction → Face Detection → ResNeXt → LSTM → Prediction → Heatmap → Web Interface

- **ResNeXt-50**: Extracts feature maps from each face image.
- **LSTM**: Learns sequential dependencies from extracted frame features.
- **Binary Classification**: Predicts Real or Fake label per video.
- **Explainability**: Grad-CAM or attention-based heatmaps overlayed.

## 📂 Dataset

We used the **Deepfake Detection Challenge Dataset (DFDC)** provided by Facebook AI.

📥 Download:  
- [DFDC Dataset on Kaggle](https://www.kaggle.com/datasets/c/dfdc-deepfake-detection-challenge)
**Note:** Due to its large size, only a subset (real + fake videos) was used during training. Face frames were extracted and saved using a custom face extraction pipeline.
📈 Results
Metric	Value
Accuracy	92.5%
F1-Score	0.91
Model Size	~180 MB
Test Dataset	DFDC Subset

✅ Successfully classified unseen deepfake videos

🤝 Contributing
We welcome contributions! To contribute:

Fork the repository.

Create a new branch.

Make your changes.

Submit a pull request.

🚀 Deployment Note
⚠️ Notice:
This deepfake detection system has been deployed for a limited short-term demonstration.
We plan to enhance, scale, and host it permanently on cloud platforms (like AWS, GCP, or Azure) to make it accessible to a wider audience in the near future.
Stay tuned for updates and improved real-time detection features!
