# 📊 TOPSIS Implementation in Python

This project implements the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method using Python. It helps in solving multi-criteria decision-making problems by ranking alternatives based on their distance from the ideal solution.

---

## 🚀 Features
- 📁 Supports CSV input
- ⚖️ Custom weights and impacts
- 🧮 Complete TOPSIS calculation
- 📊 Generates ranking with scores
- 📝 Available in:
  - Python Script (`topsis.py`)
  - Jupyter Notebook (`topsis_analysis.ipynb`)
- ❌ Strong error handling & validation

---

## 📂 Project Structure
```
├── topsis.py                 # Command-line implementation
├── topsis_analysis.ipynb     # Notebook version (step-by-step)
├── data.csv                  # Sample dataset
└── README.md                 # Documentation
```

---

## 🧠 What is TOPSIS?

TOPSIS stands for **Technique for Order Preference by Similarity to Ideal Solution**.

👉 Idea:
- Best option = Closest to **ideal best**
- Worst option = Farthest from **ideal worst**

---

## 🔄 Algorithm Steps
1. Normalize the decision matrix  
2. Apply weights  
3. Determine ideal best & worst  
4. Calculate distance from ideal points  
5. Compute TOPSIS score  
6. Rank alternatives  

---

## ⚙️ Requirements

Install dependencies:

```bash
pip install pandas numpy
```

---

## ▶️ Usage (Python Script)

```bash
python topsis.py <InputDataFile> <Weights> <Impacts> <OutputResultFile>
```

### ✅ Example:
```bash
python topsis.py data.csv "1,1,1,1" "+,+,-,+" result.csv
```

---

## 📓 Usage (Jupyter Notebook)

Open the notebook:

```bash
jupyter notebook topsis_analysis.ipynb
```

✔ Step-by-step explanation  
✔ Easy to understand  
✔ Great for learning & demo  

---

## 📥 Input File Format
- CSV file  
- Minimum **3 columns required**  
- First column → Non-numeric (e.g., names)  
- Remaining columns → Numeric values  

### Example:
```
Model,Price,Quality,Durability,Performance
A,25000,7,8,9
B,30000,8,7,8
C,28000,9,6,7
```

---

## ⚖️ Parameters

### Weights
- Comma-separated numbers  
- Example: `"1,2,3,4"`

### Impacts
- `+` → Beneficial criteria  
- `-` → Non-beneficial criteria  
- Example: `"+,+,-,+"`

---

## 📤 Output
The output CSV includes:
- Original data  
- ⭐ **Topsis Score**  
- 🏆 **Rank (Higher score = better rank)**  

---

## ❌ Error Handling
Handles:
- Missing/invalid file  
- Non-numeric data  
- Mismatched weights & impacts  
- Invalid impact symbols  

---

## 💡 Use Cases
- 📱 Product comparison  
- 🎓 College selection  
- 💼 Business decisions  
- 📊 Multi-criteria optimization  

---

## 🛠️ Tech Stack
- Python  
- Pandas  
- NumPy  

---

