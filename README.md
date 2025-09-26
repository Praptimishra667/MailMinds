# 📧 MailMinds  

**MailMinds** is an AI-powered cold email generator for services companies, built with **Groq**, **LangChain**, and **Streamlit**.  

It enables users to input the URL of a company's **careers page**, automatically extracts job listings, and generates **personalized cold emails** tailored to those roles. The generated emails are enriched with **portfolio links** sourced from a vector database, ensuring relevance to the specific job descriptions.  

---

## 🚀 Why MailMinds?  

Hiring can be time-consuming and resource-heavy. Companies spend valuable effort on:  
- Screening candidates  
- Conducting interviews  
- Onboarding new employees  
- Training fresh hires  

With **MailMinds**, service-based companies can **bridge the gap** by reaching out to potential clients directly, offering dedicated experts that fit their hiring needs.  

💡 **Example Scenario:**  
Nike is hiring a **Principal Software Engineer**. Instead of waiting through the traditional hiring cycle, **Atliq** (a software services provider) can directly offer a dedicated software engineer to Nike.  
The business development executive (**Mohan**) from Atliq uses **MailMinds** to craft a **personalized cold email** to Nike, showcasing relevant portfolios and expertise.  

---

## 🏗 Architecture  

![Architecture Diagram](img.png)  

---

## ✨ Features  

- 🔗 **Career Page Scraper** → Extracts job descriptions from company websites  
- 🤖 **AI-powered Email Generation** → Uses Groq + LangChain to generate personalized cold emails  
- 📂 **Portfolio Integration** → Retrieves relevant portfolio/project links from a vector database  
- 🎨 **Interactive UI** → Built with Streamlit for easy use  
- ⚡ **Fast & Scalable** → Powered by Groq inference for speed  

---

## 🛠 Tech Stack  

- **Python 3.9+**  
- [LangChain](https://www.langchain.com/) – for orchestration of LLM workflows  
- [Groq API](https://console.groq.com/) – for fast inference  
- [Streamlit](https://streamlit.io/) – for UI  
- [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/) – for job listings scraping  
- [FAISS / ChromaDB] – for vector database portfolio retrieval  

---

## ⚙️ Set-up  

### 1. Clone the repository  
```bash
git clone https://github.com/your-username/mailminds.git
cd mailminds
```

### 2. Get your API Key  
- Sign up and generate an API key from [Groq Console](https://console.groq.com/keys).  
- Create a `.env` file inside the `app/` directory and add:  

```env
GROQ_API_KEY=your_api_key_here
```

### 3. Install dependencies  
```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit app  
```bash
streamlit run app/main.py
```  

---

## 📖 Usage  

1. Launch the Streamlit app.  
2. Enter the **URL of a company’s careers page**.  
3. Wait for MailMinds to:  
   - Scrape job listings  
   - Generate personalized cold emails  
   - Include portfolio links  
4. Copy or send the generated email directly from the interface.  

---

## 📂 Project Structure  

```
mailminds/
│── app/
│   ├── main.py          # Streamlit app entry point
│   ├── utils.py         # Helper functions
│   ├── email_templates/ # Email templates
│   ├── vector_db/       # Portfolio embeddings
│   └── .env             # API key storage
│
│── requirements.txt     # Dependencies
│── README.md            # Documentation
│── img.png              # Architecture diagram
```

---

## 📜 License  

This software is licensed under the **MIT License**.  

⚠️ However, **commercial use of this software is strictly prohibited** without prior written permission from the author.  
Attribution must be given in all copies or substantial portions of the software.  

---

## 🤝 Contribution  

Contributions are welcome! 🚀  

1. Fork the repository  
2. Create a new branch (`feature/your-feature`)  
3. Commit your changes  
4. Open a Pull Request  

---

✍️ **Made by Prapti Mishra**  
