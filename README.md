# rocov2-image-captioning
Dissertation

# Automated Medical Image Captioning Using CNN-LSTM with Attention

A medical image captioning system that generates short descriptive captions 
for radiology images. The model uses a ResNet-50 CNN encoder, Bahdanau soft 
attention, and an LSTM decoder, trained and evaluated on the ROCOv2 dataset.

## Requirements

This project is designed to run in Google Colab with a GPU runtime.  
All required libraries are installed automatically at the top of the notebook.

## How to Run

### 1. Open in Google Colab
Download the `main.ipynb` file from GitHub, then upload
to [colab.research.google.com](https://colab.research.google.com).

### 2. Enable GPU
In Colab: `Runtime` → `Change runtime type` → set Hardware accelerator to `T4 GPU`.

### 3. Mount Google Drive
The notebook saves all data, checkpoints, and outputs to Google Drive so that 
nothing is lost when the Colab session ends. When prompted, authorise access 
to your Google Drive.

### 5. Run all cells
Run the notebook from top to bottom (`Runtime` → `Run all`).  
On the first run, the ROCOv2 dataset will be downloaded automatically 
via Hugging Face Datasets. This may take several minutes.  
Subsequent runs will load from Drive and skip the download. The training cell may take around 2 hours to run.
