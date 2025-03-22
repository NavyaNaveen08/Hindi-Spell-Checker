# N-gram & Levenshtein Hindi Spell Checker  

##  Overview  
This project implements a **spell-checking system for Hindi text** using **N-gram language models** and **Levenshtein distance**.  
The system identifies spelling errors, introduces artificial typos for evaluation, and corrects them using a **hybrid approach** combining **probabilistic n-gram models** with **edit distance techniques**.  

##  Features  
✅ Processes multiple **Hindi text datasets** and extracts words.  
✅ Generates **bigrams, trigrams, and four-grams** for probability-based predictions.  
✅ Uses **Levenshtein Distance** to suggest correct words.  
✅ Introduces **artificial typos** for evaluating spell correction accuracy.  
✅ Implements a **hybrid correction method** combining n-gram probabilities with edit distance.  
✅ Calculates **spell-checking accuracy** across different test sizes.  

##  Dataset  
>  **Note**: The datasets used for this project are **not uploaded** to this repository due to **storage constraints and privacy considerations**.  

If you wish to run the code, please use your own **Hindi text datasets** and update the file paths in the script accordingly.  

## ⚙️ Implementation Details  
🔹 **Text Preprocessing**: Reads Hindi text, removes special characters, and tokenizes words.  
🔹 **N-gram Probability Calculation**:  
&nbsp;&nbsp;&nbsp;&nbsp; Unigrams, bigrams, trigrams, and four-grams are computed.  
&nbsp;&nbsp;&nbsp;&nbsp; Probabilities are derived based on relative frequency in lower-order n-grams.  
🔹 **Error Simulation**: Introduces typos using random operations (**replace, swap, delete, insert**).  
🔹 **Spell Correction**:  
&nbsp;&nbsp;&nbsp;&nbsp; **Levenshtein Distance-based correction**: Finds the closest match from the dataset.  
&nbsp;&nbsp;&nbsp;&nbsp; **Hybrid Correction (N-gram + Levenshtein)**: Selects the best candidate using a weighted scoring system.  
🔹 **Performance Evaluation**: Accuracy is measured across different test sizes (**50, 100, 200 words**).  

##  Dependencies  
Ensure you have the following installed before running the script:  
- Python 3.x  
- NLTK  
- Collections  
- Random  
- Regex (`re`)  

Install dependencies using:  
```bash
pip install nltk  
