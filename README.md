
# Intelligent Assignment Evaluator using GenAI and LLM

An advanced **Intelligent Assignment Evaluator** leveraging **Generative AI (GenAI)** and **Large Language Models (LLM)** to automatically assess and evaluate assignments. The system utilizes **Gemini API** for extracting text from images and PDFs, including **handwritten text**, and integrates with **Generative AI** for precise grading, feedback generation, and similarity analysis.

---

## Features

- **Handwritten Text Extraction**: Uses **Gemini API** for OCR (Optical Character Recognition) to extract text from images or PDF files containing handwritten assignments.
- **Automated Grading**: Utilizes **Generative AI** to evaluate and grade the content based on predefined evaluation criteria.
- **Feedback Generation**: Automatically generates personalized feedback for students based on their assignment content.
- **Similarity Detection**: Uses **LLM** to compare assignments for plagiarism or similarity against a set of reference materials.
- **Scalable and Efficient**: Designed to handle large datasets and work seamlessly in a production environment with integrated **MLOps** concepts.

---

## Technologies Used

- **Gemini API**: For extracting text from images/PDFs of handwritten assignments.
- **Generative AI (GenAI)**: For automated grading, content analysis, and feedback generation.
- **Large Language Models (LLM)**: For similarity analysis, content understanding, and NLP tasks.
- **Python**: The main programming language for backend logic and API integration.
- **Flask/Django**: For API endpoints (optional, depending on your setup).
- **Pandas, NumPy**: For data handling and preprocessing.
- **Git**: For version control and project collaboration.

---

## Installation

Follow these steps to set up and run the project locally.

### 1. Clone the repository

```bash
git clone https://github.com/prabhakarsharma-pythonaire/Intelligent-assignment-evaluator-using-lGenai-and-llm.git


### 2. **Navigate to the project directory**
bash
Copy code
cd Intelligent-assignment-evaluator-using-lGenai-and-llm


### 3. **Set up a virtual environment**
Create and activate a virtual environment to isolate dependencies.


Copy code
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\\Scripts\\activate`


4. Install the required dependencies
Use pip to install all the necessary Python libraries.

bash
Copy code
pip install -r requirements.txt
5. Set up Gemini API Key
To use the Gemini API for text extraction, you need to set up your Gemini API key.

Obtain your Gemini API key from Gemini API.
Store your key in an environment variable for security.
bash
Copy code
export GEMINI_API_KEY='your_gemini_api_key_here'
Or, you can add it to your .env file (use a Python package like python-dotenv to load it).

Usage
1. Extract Text from Handwritten Assignment
Use the Gemini API to extract text from scanned assignment PDFs or image files:

python
Copy code
from gemini_api import extract_text_from_image

file_path = 'path_to_assignment.pdf'  # Replace with the actual file path
text = extract_text_from_image(file_path)

print(text)
2. Evaluate Assignment
After extracting the text, pass the content to the Generative AI model for automated evaluation and feedback generation.

python
Copy code
from gen_ai import evaluate_assignment

evaluation = evaluate_assignment(text)
print("Grade:", evaluation['grade'])
print("Feedback:", evaluation['feedback'])
3. Similarity Check
Use LLM to check the similarity of the assignment against other reference texts or documents:

python
Copy code
from similarity_checker import check_similarity

similarity_score = check_similarity(text, 'reference_document.txt')
print(f"Similarity Score: {similarity_score}")
Example Workflow
Extract Text: Use Gemini API to convert an assignment PDF/image into text.
Grading: Use GenAI to grade the assignment and generate feedback based on its content.
Similarity Check: Compare the student's work with a reference answer sheet or other submissions to detect plagiarism or similarity.
Contributing
Fork the repository.
Clone your fork to your local machine.
Create a new branch for your changes.
Make your changes and commit them with clear messages.
Push your changes to your forked repository.
Open a pull request to the original repository.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Contact
For any questions or feedback, feel free to reach out to:

Author: Prabhakar Sharma
Email: prabhakarkumar313@gmail.com
Acknowledgments
Gemini API: For providing a powerful tool to extract text from handwritten images and PDFs.
Generative AI Models: For enabling automated grading and feedback generation.
Open Source Communities: For the various libraries and frameworks used in this project. """
Create the README.md file and write the content
with open("/content/Intelligent-assignment-evaluator-using-lGenai-and-llm/README.md", "w") as file: file.write(readme_content)

Notify that the file is saved
print("README.md file has been created successfully!")

csharp
Copy code

### Instructions:
1. Run the code above in your Google Colab environment to generate the `README.md` file.
2. The file will be saved in your project directory (i.e., `/content/Intelligent-assignment-evaluator-using-lGenai-and-llm/README.md`).
3. After the file is created, you can download it directly from Colab by running:

```python
from google.colab import files
files.download("/content/Intelligent-assignment-evaluator-using-lGenai-and-llm/README.md")
