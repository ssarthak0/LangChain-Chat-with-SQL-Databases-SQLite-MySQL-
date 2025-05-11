# 🦜 LangChain: Chat with SQL Databases (SQLite & MySQL)

This Streamlit application enables users to interact with SQL databases using natural language queries. Leveraging LangChain's SQL agent and Groq's LLMs, the app translates user questions into SQL queries, executes them, and presents the results in an intuitive chat interface.

---

## 🚀 Features

- **Natural Language to SQL**: Convert plain English questions into SQL queries.
- **Database Support**: Connect to either a local SQLite database (`student.db`) or a remote MySQL database.
- **Interactive Chat Interface**: Engage in a conversational manner with your database.
- **Session Management**: Maintains chat history for each session.
- **Secure Credentials Handling**: Input fields for API keys and database credentials are secured.

---

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the project root with the following content:

```env
GROQ_API_KEY=your_groq_api_key
```

Replace `your_groq_api_key` with your actual Groq API key.

---

## 📄 Usage

### 1. Run the Application

```bash
streamlit run app.py
```

### 2. Configure Database Connection

- **SQLite**:
  - Ensure `student.db` is present in the project directory.
  - Select "Use SQLite 3 Database - student.db" in the sidebar.

- **MySQL**:
  - Select "Connect to your MySQL Database" in the sidebar.
  - Provide the following details:
    - MySQL Host
    - MySQL User
    - MySQL Password
    - MySQL Database Name

### 3. Enter Groq API Key

Input your Groq API key in the sidebar to enable the LLM functionalities.

### 4. Start Chatting

Type your queries in natural language in the chat input box. For example:

- "Show all students enrolled in the Data Science course."
- "What is the average score in the Mathematics class?"

The application will display the corresponding SQL query and the results fetched from the database.

---

## 📁 Project Structure

```
project-root/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables
├── student.db             # SQLite database file
├── README.md              # Project documentation
```

---

## 🧾 Requirements

The application relies on the following Python packages:

```
streamlit
langchain
python-dotenv
ipykernel
langchain-community
langchain-openai
pandas
openai
langchain-groq
mysql-connector-python
SQLAlchemy
```

Ensure all dependencies are installed by running:

```bash
pip install -r requirements.txt
```

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgments

- [LangChain](https://github.com/langchain-ai/langchain) for providing the framework for building LLM applications.
- [Streamlit](https://streamlit.io/) for the interactive web interface.
- [Groq](https://groq.com/) for the language models powering the chatbot.

---

Feel free to contribute to this project by submitting issues or pull requests.
