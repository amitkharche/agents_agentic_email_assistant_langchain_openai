
---

# 📧 Agentic AI Email Assistant

**An autonomous email response system powered by Machine Learning, GPT, and LangChain Agents.**

---

## 💼 Business Use Case

In modern enterprises, manually triaging and responding to large volumes of emails—especially support or inquiry-related ones—can drain valuable time and resources.

This project solves that by creating an **Agentic AI Email Assistant** that:

* Classifies incoming emails (e.g., Support, Sales, General Inquiry)
* Crafts intelligent replies using GPT via LangChain
* Operates with minimal human intervention using autonomous agent reasoning

---

## 🧠 Key Technologies

| Component             | Role                                                                |
| --------------------- | ------------------------------------------------------------------- |
| **ML Classifier**     | Determines the intent of each email (e.g., complaint, question)     |
| **GPT-4 + LangChain** | Generates customized replies and performs reasoning using tools     |
| **Streamlit UI**      | Provides a user-friendly interface to upload, classify, and respond |
| **Agentic AI**        | Uses LangChain tools and agents to make decisions autonomously      |

---

## 🚀 Features

✅ Upload email data in `.csv` format (`sender`, `subject`, `body`)
✅ Automatically classify emails into predefined categories
✅ Generate GPT-powered replies tailored to each email's intent
✅ Download a final CSV with classification labels and generated responses
✅ Tool-augmented LangChain Agent that simulates human-like triage behavior

---

## 🛠️ Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/amitkharche/agents_agentic_email_assistant_langchain_openai.git
   cd agents_agentic_email_assistant_langchain_openai
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set your OpenAI API key**
   Create a `.env` file in the root directory:

   ```env
   OPENAI_API_KEY=your_openai_key_here
   ```

4. **Run the Streamlit app**

   ```bash
   streamlit run app/app.py
   ```

---

## 📁 Project Structure

```
agentic-ai-email-assistant/
├── app/
│   └── app.py                        # Streamlit UI entrypoint
├── src/
│   ├── inference.py                 # Email classification & reply generation
│   ├── utils.py                     # Helper functions (preprocessing, I/O)
│   └── langchain_tools.py           # Custom LangChain tools (if any)
├── models/
│   └── email_classifier.pkl         # Pretrained ML model for intent classification
├── data/
│   └── raw/
│       └── emails.csv               # Example input data
├── notebooks/
│   ├── exploratory_analysis.ipynb   # Data exploration & preprocessing
│   └── model_training_and_evaluation.ipynb  # ML model training & evaluation
├── .env                             # OpenAI key (excluded from version control)
├── requirements.txt                 # Python dependencies
├── Dockerfile                       # Optional containerization
└── README.md
```

---

## 🧠 Agentic AI Framing

This project uses **LangChain’s agent framework** (`initialize_agent`) to go beyond static prompts:

* **LangChain Tools** enable additional logic, data lookup, or transformation
* The **agent** decides which tool to invoke based on email content and task
* GPT acts autonomously to simulate realistic human decision-making in email responses

---

## 💡 Sample Workflow

1. Upload a `.csv` file with email data
2. The classifier assigns an intent label to each email
3. GPT generates a custom reply based on the label and content
4. You can preview and download the updated dataset with responses

---

## 📬 Contact

* 💼 [LinkedIn](https://www.linkedin.com/in/amit-kharche)
* ✍️ [Medium](https://medium.com/@amitkharche14)
* 💻 [GitHub](https://github.com/amitkharche)

---
