#  Installation Guide: Lung Cancer Diagnosis Using MRI and Random Forest

This guide will walk you through installing and running the Lung Cancer Diagnosis project locally on your system. The project includes:

- A Jupyter Notebook for training and evaluation  
- A Streamlit-based web app for real-time predictions

---

##  System Requirements

- Python 3.8 or above  
- Pip or Conda  
- Jupyter Notebook  
- Optional: Git (for cloning the repository)

---

## 📁 Project Folder Structure

###### lung_cancer_project/

├── dataset/    
│ ├── benign/   
│ └── malignant/   
├── lung_cancer_rf.ipynb  
├── lung_cancer_rf_model.pkl   
├── label_encoder.pkl     
├── app.py   
├── requirements.txt    
├── installation.md   
└── README.md  

###### Step 2: Create a Virtual Environment (Recommended)

🔹 Windows (CMD or PowerShell)
````
python -m venv venv
venv\Scripts\activate
````
🔹 macOS / Linux
````
python3 -m venv venv
source venv/bin/activate
````
##### Step 3: Install Python Dependencies
````
pip install -r requirements.txt
````
###### If you get errors during installation, try upgrading pip first:
````
pip install --upgrade pip
````

###  Step 4: Prepare the Dataset

##### Place your MRI images in the following format:
````
dataset/  
├── benign/  
│   └── image1.jpg, image2.jpg, ...  
└── malignant/  
    └── imageA.jpg, imageB.jpg, ...
````
##### Step 5: Run the Jupyter Notebook (Model Training & Evaluation)
````
jupyter notebook lung_cancer_rf.ipynb
````
###### Inside the notebook:

Load data

Train the Random Forest model

Evaluate with accuracy and confusion matrix

Save the model as .pkl for the GUI

##### Step 6: Launch the Streamlit App (GUI Interface)
```
streamlit run app.py
```
A browser window will open.

Upload an MRI image.

You’ll receive a malignant/benign prediction and confidence score.

# Troubleshooting

###### Problem	Solution

ModuleNotFoundError             

Ensure you installed all packages via pip install -r requirements.txt

cv2 error	

Install OpenCV: 

pip install opencv-python

Streamlit app not opening        
````
Try localhost:8501 in your browser
````
Jupyter not launching

Install it via pip install notebook

##### You're Ready!

You can now:

Train and evaluate your lung cancer classifier

Predict cancer status via the Streamlit GUI

Deploy it online or expand for CT scans, X-rays, etc.