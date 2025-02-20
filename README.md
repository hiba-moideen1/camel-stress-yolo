# Detecting Stress Parameters in Dromedary Camels Using Computer Vision
Official Implementation of the "Detecting Stress Parameters in Dromedary Camels Using Computer Vision" Paper.
**Project Description:**  
This study focuses on stress detection in dromedary camels using deep learning. Camels at the Marmoom Farm were monitored for six days under different conditions, including blood sample collection and intense training. Video footage was analyzed to build a YOLOv8-based model that detects both normal (e.g., standing, sitting, sleeping) and stress-related behaviors (e.g., distressed sitting, uncontrollable movement, rope pulling). The model achieved high accuracy, with a precision of 0.971 and recall of 0.959. By examining behavioral responses to stressors, the study provides valuable insights into camel welfare, enabling early intervention and improved management practices.

## 1. Clone the Repository
First, download the project files from GitHub

```
git clone https://github.com/hiba-moideen1/camel-stress-yolo.git
cd your-repo
```

## 2. Set Up a Virtual Environment
Create and activate a virtual environment to manage dependencies.

***For Python Virtual Environment (`venv`)***

```
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

***For Conda Environment***

```
conda create --name stress_prediction python=3.8 -y
conda activate stress_prediction
```

## 3. Install Dependencies
Check CUDA version:

```
nvcc --version
```

Install CUDA Toolkit:
```
conda install -c anaconda cudatoolkit
```

Install PyTorch:
```
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
```

Verify GPU Support:
```
import torch
print(torch.cuda.is_available())
print(torch.cuda.get_device_name(0))  # 0 corresponds to the first GPU
```


## 4. Run Jupyter Notebook
Once dependencies are installed, launch Jupyter Notebook:

```
conda install jupyter   
jupyter notebook
```
Then, open the `stress_prediction.ipynb` file.

***Dataset*** - The preprocessed dataset is embedded directly from Roboflow onto the project using the API key. 





