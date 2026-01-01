
# 🔥 hot_seat — Corporate Interview Question Generator


hot_seat is a Python-powered automated **MCQ (Multiple Choice Question) generator** built specifically for **technical & corporate hiring assessments**, not for college examination papers or student quizzes.


It retrieves topic-related information using **SERP API**, scrapes article content, processes it through a **local Phi-3 Language Model**, and generates **50 professional interview MCQs per topic**, complete with an **answer key**, exporting them as **.docx files** for direct use.


This tool is ideal for **HR teams, L&D departments, technical hiring rounds, internal corporate evaluation, and EdTech assessment platforms.**



## 🚀 Features


- Generates **50 MCQs automatically per topic**  

- Uses **SERP API** to fetch real-world content  

- Scrapes & extracts article text using BeautifulSoup  

- Feeds data into **Phi-3 model via llama.cpp**  

- Exports fully formatted **Word (.docx) question banks**  

- Perfect for workplace-grade interview preparation  



## 🎯 Intended For


| Suitable For | Not Designed For |
|-------------|------------------|
| Corporate interview prep | University exam question papers |
| Technical hiring rounds | Student assignments |
| HR/L&D assessments | Coaching material generation |
| Internal skill evaluation | Semester tests |
| EdTech integration | Basic academic quizzes |


This tool is strictly for **industry-oriented interview difficulty**, not academic syllabus question setting.  



## 🛠 Requirements


- Python **3.8+**  

- `.env` with `SERP_API_KEY`  

- `Phi-3-mini-4k-instruct-q4.gguf` model in root folder  

- Packages from `requirements.txt`  



## 🔧 Setup & Run

---> install and place the Phi-3-mini model (the one specified above) in the same folder as hot_seat.py

```bash
git clone <repo_url> hot_seat

cd hot_seat

python3 -m venv venv
source venv/bin/activate      # Mac/Linux

# OR
venv\Scripts\activate         # Windows

pip install -r requirements.txt

echo "SERP_API_KEY=your_key_here" > .env

# Edit topics.txt (one topic per line)

python3 hot_seat.py
