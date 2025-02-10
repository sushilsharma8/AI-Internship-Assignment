# AI-Internship-Assignment
## Part A: Task Extraction  
### How to Run:  
1. Install dependencies:  
   ```bash
   pip install spacy nltk gensim scikit-learn
   python -m spacy download en_web_sm
Run the code:

python
Copy
python part_a.py
Example input/output provided in sample_input.txt.

Part B: Sentiment Analysis
Dataset Setup:
Download the IMDb dataset from Stanford link.

Extract it into aclIm/ folder.

Run the:

python
Copy
python part_b.py
Results:
Accuracy: %, Precision: 88%, Recall: 89%.

Copy

---

#### 2.Validation Sample (part_a_validation.txt)**  
```plaintext
Input: "Priya must complete the slides by 5 pm tomorrow  
Output:{
  "task": "Priya must complete the slides by 5 pm tomorrow.",
  "entity": "Priya",
  "deadline": "5 pm tomorrow"
}
3. Insights & Challenges Document
Insights:

Heuristic rules (modal verbs + action verbs) effectively identify tasks.

TF-IDF captures critical features for sentiment classification.

Challenges:

Regex patterns for deadlines needed multiple iterations.

Model initially overfit due to imbalanced n-grams; resolved with max_features=5000.
