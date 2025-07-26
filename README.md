# 🧠 CSCN8010 Lab 3: Custom CNN vs VGG16 (Dogs vs Cats)

This lab explores a classification task using Convolutional Neural Networks (CNNs) to distinguish between images of dogs and cats. The lab compares a **custom-built CNN** with a **pretrained VGG16** model, tracking large model files using **Git LFS**.

---

## 📁 Project Structure

CSCN8010-Lab3/
│
├── Data/ # Contains training and validation image datasets
├── fast_custom_cnn.h5 # Saved model (custom CNN)
├── best_vgg16.h5 # Saved model (VGG16)
├── CNN_vs_VGG16.ipynb # Jupyter Notebook with all code
├── .gitattributes # Git LFS tracking rules
├── requirements.txt # Python dependencies
└── README.md # You're here!


## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/KapilBhardwaj2702/CSCN8010-Lab3.git
cd CSCN8010-Lab3
2. Install Python dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Install Git LFS (if not already)
bash
Copy
Edit
git lfs install
4. Pull large files (model weights)
bash
Copy
Edit
git lfs pull
🏗️ Models
fast_custom_cnn.h5: Trained custom CNN architecture.

best_vgg16.h5: Transfer learning using pretrained VGG16.

Both are tracked using Git LFS due to size (>100MB).

📊 Results (Sample)
| Model      | Accuracy | Loss |
| ---------- | -------- | ---- |
| Custom CNN | 85.4%    | 0.37 |
| VGG16      | 92.1%    | 0.28 |

🧪 Experiments
EarlyStopping and ModelCheckpoint callbacks used.

Data augmentation applied via ImageDataGenerator.

Evaluation includes accuracy, classification report, confusion matrix.

📦 Requirements
See requirements.txt. Key libraries:

tensorflow

matplotlib

numpy

scikit-learn

📌 Notes
.h5 files are tracked with Git LFS. GitHub will block files >100MB if not tracked correctly.

Always run git lfs pull after cloning.

🙋‍♂️ Author
Kapil Bhardwaj
Conestoga College — CSCN8010
GitHub
