**CNN-GAT-Physics-Based Single Image Dehazing**



&#x20;**Overview**



This repository contains the implementation of a hybrid CNN-GAT-Physics Based framework for single image dehazing. The proposed model integrates Convolutional Neural Networks (CNNs), Graph Attention Networks (GATs), and physics-based atmospheric scattering principles to effectively remove haze from degraded images while preserving structural and texture information.



The CNN module is responsible for extracting local image features, whereas the GAT module captures long-range spatial relationships and contextual dependencies among image regions. The physics-based component incorporates atmospheric scattering information to guide the restoration process and improve image visibility.



&#x20;**Associated Manuscript**



This repository is associated with the manuscript submitted to The Visual Computer.



&#x20;**Features**



\* Single image dehazing

\* CNN-based feature extraction

\* Graph Attention Network (GAT) integration

\* Physics-based atmospheric scattering model

\* PSNR and SSIM evaluation

\* Training and inference support



&#x20;**System Requirements**



&#x20;**Hardware**



\* Intel Core i5/i7 processor or equivalent

\* Minimum 8 GB RAM

\* NVIDIA GPU with CUDA support (recommended)



&#x20;**Software**



\* Python 3.10

\* PyTorch 2.0

\* CUDA



&#x20;**Required Libraries**



**Install dependencies using:**



pip install -r requirements.txt



Required packages include:



\* torch

\* torchvision

\* numpy

\* opencv-python

\* matplotlib

\* scikit-image

\* tqdm

\* Pillow



&#x20;**Dataset**



Experiments were conducted using publicly available image dehazing datasets.



**Recommended Dataset:**



**RESIDE Dataset**



**Dataset Link:**

https://www.kaggle.com/datasets/kmljts/reside-6k



After downloading, organize the dataset as:



dataset/

├── train/

├── test/

└── ground\_truth/



&#x20;Repository Structure



CNN-GAT-Physics-Dehazing:

**1.CNN-GAT-Physics code :**



2\. dataset



3\. outputs diagrams

4\. requirements.txt

5.README.md



Training Configuration Used in the Manuscript:



\* Epochs: 150

\* Optimizer: Adam

\* Learning Rate: 0.0001





Testing



To evaluate the trained model:



python test.py



Dehazed images will be stored in the output directory.



Evaluation Metrics

&#x20;The following metrics are used:



\* Peak Signal-to-Noise Ratio (PSNR)

\* Structural Similarity Index Measure (SSIM)



Run: python evaluate.py

**Reproducibility Note**



The results reported in the associated manuscript were obtained using a training configuration of 150 epochs. Reproduced results may vary depending on software versions, hardware configuration, random initialization, dataset preparation, and training settings.



&#x20;**Architecture**



The proposed framework consists of:



1\. CNN-based feature extraction.

2\. Graph Attention Network (GAT) for contextual feature learning.

3\. Physics-based atmospheric scattering guidance.

4\. Reconstruction module for haze-free image generation.

