# data-analyst-agent-final# Data Analyst Agent

This project is a full-stack, autonomous data analyst agent. You can upload a dataset and a list of questions, and the agent will analyze the data to provide answers, including visualizations.

-----

## 🚀 Features

  * **Autonomous Data Analysis:** Upload a dataset and questions, and the agent will automatically generate Python code to perform the analysis.
  * **Web Scraping:** If no dataset is provided, the agent can scrape data from URLs.
  * **Visualization:** The agent can generate and display plots and charts.
  * **Frontend Interface:** A simple, user-friendly web interface for uploading files and viewing results.
  * **Robust LLM Fallback:** Uses a hierarchy of Gemini models to ensure reliability.

-----

## 🛠️ Technologies Used

  * **Backend:** FastAPI, LangChain, Google Generative AI
  * **Frontend:** HTML, CSS, JavaScript
  * **Data Science:** Pandas, NumPy, Matplotlib, Seaborn
  * **Deployment:** Docker, Uvicorn

-----

## ⚙️ Setup and Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/shreeramiitm/data-analyst-agent-final.git
    cd data-analyst-agent-final
    ```

2.  **Set up your environment:**
    Create a `.env` file and add your Gemini API keys:

    ```
    gemini_api_1=YOUR_API_KEY_1
    gemini_api_2=YOUR_API_KEY_2
    # Add up to 10 keys
    ```

3.  **Build and run with Docker:**

    ```bash
    docker build -t data-analyst-agent .
    docker run -p 8000:8000 -v $(pwd):/app data-analyst-agent
    ```

    The application will be available at `http://localhost:8000`.

-----

## Usage

1.  **Prepare your questions file:**
    Create a `.txt` file with a list of questions you want to ask about your data.

2.  **Upload your files:**

      * Open the web interface in your browser.
      * Upload your questions file.
      * Optionally, upload a dataset (CSV, Excel, Parquet, or JSON).

3.  **Analyze and get results:**

      * Click the "Analyze Data" button.
      * The agent will process your request and display the answers, including any generated plots.

-----

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
