# 🍳 Smart Recipe Generator

This project is a **FastAPI-based Smart Recipe Generator** that predicts ingredients from an image and generates corresponding recipes using AI models.  

## Project link : https://lovable-ai-kitchen-86.vercel.app/

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/b839b6ad-1c44-45d0-9845-5329b2eb7fec" />
<img width="500" height="700" alt="image" src="https://github.com/user-attachments/assets/f9af619d-4fb6-4241-b3a9-38fc5357ee9b" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d9c5724c-9f85-4966-a3b8-d13a1d86bc65" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/ae3a9d47-1c9d-442b-96f7-e004ae68be82" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d0f89ad2-df97-49b4-b771-33f6846cf43e" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/f94d0235-7101-4b07-80d7-d01fbcb3b0c2" />


---

## 🚀 Features

- Upload food images and extract ingredients using AI.
- Generate recipes automatically using a generative AI model.
- RESTful API built with **FastAPI**.
- Interactive API documentation with **Swagger UI**.
- Modular code structure (API, Services, Models, etc).

---

## 🛠️ Tech Stack

- **Backend:** Python, FastAPI, Uvicorn  
- **AI Models:** CLIP / ResNet for image feature extraction, Llama / GPT for text generation  
- **Environment:** Virtual Environment (venv)  
- **Package Manager:** pip  

---

## ⚙️ Setup Instructions

Follow the steps below to set up and run the project:

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/SmartRecipeGenerator.git
cd SmartRecipeGenerator
```
### 2️⃣ Create and Activate Virtual Environment
# Create virtual environment
python -m venv venv

# Activate it (Windows)
venv\Scripts\activate

# (Mac/Linux)
source venv/bin/activate

### 3️⃣ Install All Dependencies
```
pip install -r requirements.txt
```
If you encounter ModuleNotFoundError, manually install the missing package:
```
pip install fastapi uvicorn fireworks-ai pillow torch torchvision transformers
```
### 4️⃣ Run the FastAPI Application
```
uvicorn main:app --reload
```
### 🌐 Access the App locally at
```
👉 http://127.0.0.1:8000
```
### 🧠 Troubleshooting

If you face errors like missing modules:
```
pip install -r requirements.txt
```
To deactivate the virtual environment:
```
deactivate
```
If you face issues related to fireworks.client:
```
pip install fireworks-ai
```

### Example Commands (Quick Run)
```
cd recipeGen-main
venv\Scripts\activate
uvicorn main:app --reload
```
## 📦 Directory Structure
<details> <summary>📁 Click to expand the copyable version</summary>
recipeGen-main/
│
├── api/
│ ├── init.py
│ ├── api.py
│ └── endpoints/
│ ├── image.py
│ ├── generative.py
│ ├── recipes_kaggle.py
│ └── image_generation.py
│
├── crud/
│ ├── init.py
│ └── crud_recipe.py
│
├── db/
│ ├── init.py
│ └── mongodb.py
│
├── models/
│ └── init.py
│
├── services/
│ ├── init.py
│ └── imgGen.py
│
├── main.py
├── requirements.txt
└── README.md
</details>

### 🧩 Future Scope

Add multilingual recipe generation
Enable nutritional value prediction
Enhance image-to-ingredient accuracy
Add voice-based recipe instructions

### 🏁 Conclusion
This project demonstrates how AI can assist in food recognition and recipe generation through an efficient and explainable pipeline using FastAPI and deep learning models.
