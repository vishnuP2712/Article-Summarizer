<h1>Article Summarizer 📰</h1>

<p>This Python script fetches a news article from a given URL, extracts its main text content, and then uses a pre-trained model from the Hugging Face Transformers library to generate a concise summary.</p>

<h2>How It Works ⚙️</h2>
<p>The script performs the following steps:</p>
<h3>📲 Fetch Content</h3>
<p>Utilizes the requests library to send an HTTP GET request to the target URL and retrieve the raw HTML of the webpage.</p>
<h3>🧹 Parse HTML</h3>
<p>Employs BeautifulSoup to parse the complex HTML structure. It specifically targets paragraph tags to extract the main body of the article, filtering out ads, navigation bars, and other irrelevant content.</p>
<h3>🧠 Generate Summary</h3>
<p>The extracted text is passed to a summarization pipeline from Hugging Face Transformers. By default, it uses the sshleifer/distilbart-cnn-12-6 model, which is fine-tuned for summarizing news articles.</p>
<h3>📄 Display Output</h3>
<p>The final, condensed summary is printed neatly to the console for the user to read.</p>

<h2>Prerequisites 🛠️</h2>
<p>Before running the script, you need to have Python 3 installed. You will also need to install the necessary libraries.</p>
<ul>
    <li><b>requests:</b> For making HTTP requests to the article URL.</li>
    <li><b>beautifulsoup4:</b> For parsing the HTML content.</li>
    <li><b>transformers:</b> For using the summarization pipeline from Hugging Face.</li>
    <li><b>torch:</b> The backend framework for the summarization model.</li>
</ul>

<h2>Usage 🚀</h2>
<p><b>Step 1:</b> Clone this repository or save the script file (summarize_article.py) to your local machine.</p>
<p><b>Step 2:</b> Open your terminal or command prompt.</p>
<p><b>Step 3:</b> Navigate to the directory where you saved the file.</p>
<p><b>Step 4:</b> Run the script using the following command: ➡️ <code>python summarize_article.py</code></p>
<p><code>Please enter the article URL and press Enter: [YOUR_ARTICLE_URL_HERE]</code></p>
<p><b>NOTE:</b> When prompted, paste the full URL of the news article you want to summarize and press Enter.</p>
