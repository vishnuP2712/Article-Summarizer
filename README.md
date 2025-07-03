Article Summarizer 📰
 
This Python script fetches a news article from a given URL, extracts its main text content, and then uses a pre-trained model from the Hugging Face Transformers library to generate a concise summary.

How It Works ⚙️

The script performs the following steps:

📲 Fetch Content: Utilizes the requests library to send an HTTP GET request to the target URL and retrieve the raw HTML of the webpage.

🧹 Parse HTML: Employs BeautifulSoup to parse the complex HTML structure. It specifically targets paragraph tags to extract the main body of the article, filtering out ads, navigation bars, and other irrelevant content.

🧠 Generate Summary: The extracted text is passed to a summarization pipeline from Hugging Face Transformers. By default, it uses the sshleifer/distilbart-cnn-12-6 model, which is fine-tuned for summarizing news articles.

📄 Display Output: The final, condensed summary is printed neatly to the console for the user to read.

Prerequisites 🛠️

Before running the script, you need to have Python 3 installed. You will also need to install the necessary libraries.

requests: For making HTTP requests to the article URL.

beautifulsoup4: For parsing the HTML content.

transformers: For using the summarization pipeline from Hugging Face.

torch: The backend framework for the summarization model.

Usage 🚀

Clone this repository or save the script file (summarize_article.py) to your local machine.
Open your terminal or command prompt.
Navigate to the directory where you saved the file.
Run the script using the following command:
➡️ python summarize_article.py

Please enter the article URL and press Enter: [YOUR_ARTICLE_URL_HERE]

NOTE: When prompted, paste the full URL of the news article you want to summarize and press Enter.
