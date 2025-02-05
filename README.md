# **Linguistic Task Extractor (LTE)**

## **Overview**
Linguistic Task Extractor (LTE) is a heuristic-based Natural Language Processing (NLP) pipeline designed to extract actionable tasks from unstructured text. It identifies sentences representing tasks, extracts details like the responsible person (assignee) and deadlines, and categorizes tasks into predefined categories such as "Development," "Documentation," and "Maintenance."

This project is particularly useful for task management systems, enabling users to process and organize unstructured information efficiently.

---

## **Features**
- **Task Identification**: Extract actionable sentences containing tasks from unstructured text.
- **Entity Extraction**: Identify the person or entity responsible for the task.
- **Deadline Detection**: Extract deadlines or time-related information from text.
- **Task Categorization**: Dynamically assign tasks to categories such as:
  - Development
  - Documentation
  - Purchase
  - Maintenance
  - Communication
- **Preprocessing**: Includes text cleaning, tokenization, and lemmatization.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries and Frameworks**:
  - `spaCy`: For sentence tokenization and Named Entity Recognition (NER).
  - `NLTK`: For POS tagging and tokenization.
  - `Regex (re)`: For deadline extraction.
  - `WordNetLemmatizer`: For lemmatization.

---

## **Setup and Installation**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/tejash-300/Linguistic-Task-Extractor.git
   cd Linguistic-Task-Extractor
   ```

2. **Install Dependencies**:
   Ensure you have Python installed. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download Required NLTK Data**:
   Run the following script to download essential NLTK datasets:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('stopwords')
   nltk.download('wordnet')
   ```

4. **Download spaCy Model**:
   ```bash
   python -m spacy download en_core_web_sm
   ```

---

## **Usage**

1. **Input Text**: Provide a paragraph of unstructured text.
2. **Run the Script**:
   ```bash
   python linguistic_task_extractor.py
   ```
3. **Output**: A structured list of tasks with details:
   - Task description
   - Assignee
   - Deadline
   - Category

Example Input:
```
Rahul has to buy snacks for the team. Sarah must complete the project report by Friday.
```

Example Output:
```
Task 1:
- Description: Rahul has to buy snacks for the team.
- Assignee: Rahul
- Deadline: Not specified
- Category: Purchase

Task 2:
- Description: Sarah must complete the project report by Friday.
- Assignee: Sarah
- Deadline: Friday
- Category: Documentation
```


## **Future Enhancements**
- Incorporate machine learning models for improved task categorization.
- Add multi-language support for broader usability.
- Develop a web-based interface for easier interaction and visualization.
- Integrate with project management tools like Trello or Asana.

---

## **Contributing**
Contributions are welcome! Please fork the repository and submit a pull request for any features or bug fixes.


## **Contact**
If you have any questions or suggestions, feel free to reach out:
- **Email**: tejashpandey740@gmail.com
- **GitHub**: [tejash-300](https://github.com/tejash-300)

---

Feel free to modify this template as per your project specifics!
