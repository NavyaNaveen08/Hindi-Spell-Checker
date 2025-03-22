## **N-gram Statistical Language Model (SLM) for Hindi Spell Checking**  

## **Overview**  
This project develops a **Statistical Language Model (SLM)** for **spell-checking Hindi text** using **bigram, trigram, and 4-gram models**. The system evaluates its performance on a test set of **50 words**, using accuracy as the evaluation metric.  

## **Tasks Performed**  
✔ **Developed N-gram SLMs**:  
- **Bigram Model**  
- **Trigram Model**  
- **4-gram Model**  

✔ **Evaluated Model Performance**:  
- Introduced artificial typos to test spell correction.  
- Measured **accuracy** as:  
  \[
  \text{Accuracy} = \frac{\text{Total Correct Spellings}}{\text{Total Words Tested (50)}}
  \]  

✔ **Implemented Spell Correction Techniques**:  
- **Levenshtein Distance**: Finds the closest correct word.  
- **Hybrid Correction**: Combines n-gram probabilities with edit distance.  

## **Dataset**  
⚠ **Note**: The dataset used for training is **not uploaded** due to privacy issues.  

## **Implementation Details**  
### **1️⃣ Preprocessing**  
- Reads Hindi text from multiple datasets.  
- Removes special characters and tokenizes words.  

### **2️⃣ N-gram Probability Calculation**  
- Computes **unigrams, bigrams, trigrams, and 4-grams**.  
- Estimates word probabilities for correction suggestions.  

### **3️⃣ Spell Correction Methods**  
- **Levenshtein Distance**: Matches words based on edit distance.  
- **Hybrid Approach**: Uses both **edit distance & n-gram probabilities**.  

### **4️⃣ Performance Evaluation**  
- **Evaluated on 50 words with typos**.  
- **Accuracy metric** used for comparison.  

## **Dependencies**  
 **Python 3.x**  
 **NLTK**  
 **Collections**  
 **Random**  
 **Regex (`re`)**  

 Install dependencies using:  
```bash
pip install nltk
```  

## **Usage**  
Run the script:  
```bash
python spell_checker.py
```  

## **Results & Accuracy**  
The model reports accuracy for **bigram, trigram, and 4-gram spell-checking methods**, helping to analyze their effectiveness in Hindi text correction.  
