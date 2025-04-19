# ChatAnalyzer: Uncover Insights from Your WhatsApp Chats

ChatAnalyzer processes your exported WhatsApp chat data to reveal communication patterns, vocabulary usage, engagement metrics, and temporal trends. This application transforms raw conversation data into insightful visual representations, allowing you to discover hidden patterns in your digital communications.

## Features

* **Data Import & Processing:** Supports common WhatsApp chat export formats (usually `.txt` files).
* **Statistical Analysis:** Provides message counts, word frequency analysis, and response pattern identification.
* **Visual Representations:**
    * Word clouds of the most frequently used words.
    * Message frequency timeline visualizations (daily, weekly).
    * Analysis and visualization of word usage over time.
    * Conversation activity heatmaps showing peak interaction times.

## 🛠️ Technology Stack

* **Backend:** Python with powerful data processing libraries like Pandas and NumPy.
* **Data Visualization:** Utilizes Matplotlib, Wordcloud, and Plotly for creating informative visuals.
* **Deployment:** Includes Heroku-ready configuration for easy online deployment.

## 🚀 Getting Started

### Prerequisites

* Python 3.7+ installed on your system.
* `pip` (Python package installer) should be up to date.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/ChatAnalyzer.git](https://github.com/yourusername/ChatAnalyzer.git)
    cd ChatAnalyzer
    ```
    *(Replace `https://github.com/yourusername/ChatAnalyzer.git` with the actual repository URL)*

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    This command will install all the necessary Python libraries listed in the `requirements.txt` file (pandas, numpy, matplotlib, wordcloud, plotly).

3.  **Run the application:**
    ```bash
    python app.py
    ```
    This command will start the ChatAnalyzer application (assuming `app.py` is the main script). Follow the on-screen instructions to upload and analyze your chat data.

## Usage

1.  **Export your WhatsApp chat data:**
    * Open the specific chat in WhatsApp you want to analyze.
    * Tap the three vertical dots (menu) in the top right corner.
    * Select "More" and then "Export chat".
    * Choose whether to include media or export without media. The application primarily analyzes text data, so exporting without media is usually sufficient.
    * Save the exported `.txt` file to a location accessible by the ChatAnalyzer application.

2.  **Load the data into ChatAnalyzer:**
    * Run the `app.py` script.
    * The application will likely provide a user interface (either command-line or web-based) where you can upload or specify the path to your exported `.txt` file.

3.  **Generate visualizations and insights:**
    * Follow the prompts within the application to initiate the analysis.
    * ChatAnalyzer will process the data and generate the various visualizations and statistical summaries.

4.  **Interpret the results:**
    * Examine the generated word clouds to understand the most frequent terms used in the conversation.
    * Analyze the message frequency timelines to identify periods of high and low activity.
    * Observe the word usage patterns over time to see how vocabulary might have evolved.
    * Study the conversation activity heatmaps to pinpoint the times of day or days of the week with the most interaction.

## Deployment

This project includes configuration files (like `Procfile`) for deployment on Heroku, a platform for deploying and managing web applications. Follow these steps to deploy ChatAnalyzer:

1.  **Create a Heroku account and install the Heroku CLI:**
    * Go to [https://www.heroku.com/](https://www.heroku.com/) and sign up for an account if you don't have one.
    * Download and install the Heroku Command Line Interface (CLI) from [https://devcenter.heroku.com/articles/heroku-cli](https://devcenter.heroku.com/articles/heroku-cli).

2.  **Login to Heroku and create a new app:**
    * Open your terminal or command prompt and log in to Heroku:
        ```bash
        heroku login
        ```
    * Follow the prompts to enter your Heroku credentials.
    * Create a new Heroku application:
        ```bash
        heroku create your-app-name
        ```
        *(Replace `your-app-name` with a unique name for your application)*

3.  **Connect your GitHub repository to Heroku:**
    * Navigate to your application's dashboard on the Heroku website.
    * Go to the "Deploy" tab.
    * Under "Deployment method," choose "GitHub."
    * Search for your repository (`yourusername/ChatAnalyzer`) and click "Connect."

4.  **Deploy the application:**
    * Once connected, you have a few options for deployment:
        * **Automatic Deploys:** Enable automatic deploys from your `main` (or specified) branch. Heroku will automatically build and deploy your application whenever you push changes to that branch.
        * **Manual Deploy:** Click the "Deploy Branch" button under the "Manual Deploy" section to manually deploy the latest version of your code.

    * Heroku will build your application based on the `requirements.txt` file and the `Procfile` (which specifies how to run your Python application). Once the build is successful, your ChatAnalyzer application will be live at the Heroku-provided URL.

**Note:** You might need to adapt the `app.py` script and potentially create a web interface (using frameworks like Flask or Streamlit) to make the application user-friendly for deployment on Heroku. The current description suggests a command-line interface, which might require further development for a seamless web deployment.
