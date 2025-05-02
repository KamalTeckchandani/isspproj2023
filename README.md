**Medical-Policy-Analysis-GenAI-Prototype**
AI-Powered Medical Policy Comparison Engine

🧠 **Overview**

Medical-Policy-Analysis-GenAI-Prototype is a Generative AI-based solution that automates the comparative analysis of medical policies from various insurance providers such as Aetna, Anthem, Cigna, and more. It leverages Large Language Models (LLMs) and prompt engineering techniques to streamline document understanding, reduce manual review time, and provide intelligent insights.

Built using OpenAI APIs, Streamlit, and Amazon S3 for cloud document management, this prototype demonstrates the potential of GenAI in revolutionizing healthcare policy analysis.

🚀 **Features**

🔍 Automated Policy Parsing: Extracts and interprets content from medical policy documents (PDF/HTML).

🧾 Comparative Analysis: Generates structured comparisons across multiple providers on a given medical treatment or condition.

🧠 LLM Integration: Utilizes OpenAI's GPT models with custom prompt engineering.

☁️ Amazon S3 Integration: Fetches the latest medical policies from secure S3 buckets.

🖥️ Streamlit Interface: Intuitive UI for user inputs, policy selection, and viewing side-by-side analysis.

📂 **Architecture**

         +----------------------+
                |  Amazon S3 Bucket    |
                |  (PDFs, HTML, Docs)  |
                +----------+-----------+
                           |
                 Fetch Latest Documents
                           |
                           v
                +----------------------+
                |  Preprocessing Layer |
                | (Text extraction,    |
                |  Cleaning, Struct.)  |
                +----------+-----------+
                           |
                           v
                +----------------------+
                |   Prompt Engineering |
                |   (Dynamic templates)|
                +----------+-----------+
                           |
                           v
                +----------------------+
                | OpenAI GPT (LLMs)    |
                | Comparative Output   |
                +----------+-----------+
                           |
                           v
                +----------------------+
                |   Streamlit Frontend |
                +----------------------+

                
⚙️ **Tech Stack**

Language Model: OpenAI GPT-4

Frontend: Streamlit (Python)

Backend: Python

Cloud Storage: Amazon S3

Libraries:

boto3 (S3 integration)

PyMuPDF, pdfplumber or BeautifulSoup (document parsing)

langchain or custom prompt templating (for prompt engineering)

📈 **Use Case Example**

“Compare the prior authorization requirements for MRI scans across Aetna, Anthem, and UnitedHealthcare.”

Output: Structured tabular comparison summarizing:

Approval timelines

Medical necessity clauses

Provider network constraints

CPT codes mentioned

▶️ **Getting Started**

Clone the Repo:

git clone https://github.com/your-username/Medical-Policy-Analysis-GenAI-Prototype.git
cd Medical-Policy-Analysis-GenAI-Prototype
Install Requirements:

pip install -r requirements.txt
Configure Environment:

Set up .env for OpenAI and AWS keys

OPENAI_API_KEY=your_key
AWS_ACCESS_KEY_ID=your_key
AWS_SECRET_ACCESS_KEY=your_secret
S3_BUCKET_NAME=your_bucket

Launch App:
streamlit run main.py

📌 **Future Enhancements**

Integrate OCR for scanned documents.

Enable document version tracking.

Support additional providers and policy formats.

Export comparative reports to PDF/CSV.

👥 
Powered by OpenAI and AWS

📬 **Contact If you like the project or want to collaborate, feel free to connect:**

GitHub: (https://github.com/KamalTeckchandani)

LinkedIn: https://www.linkedin.com/in/kamal-teckchandani/
