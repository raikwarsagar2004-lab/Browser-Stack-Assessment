📘 BrowserStack Assignment – Selenium Automation
📌 Overview

This project demonstrates end-to-end Selenium automation combined with web scraping, API integration, text processing, and cross-browser testing using BrowserStack.

The solution performs the following tasks:

Scrapes opinion articles from the Spanish news website El País

Extracts article titles, content, and image captions

Translates Spanish titles into English

Performs keyword frequency analysis on translated titles

Executes cross-browser tests on BrowserStack using parallel sessions

🛠️ Tech Stack
Category	Technology
Language	Python 3
Automation	Selenium 4
Translation	googletrans (Google Translate API wrapper)
Cloud Testing	BrowserStack
Environment Management	python-dotenv
📂 Project Structure
browserstack-assignment/
│
├── main.py                 # Main script (scraping, translation, analysis)
├── browserstack_run.py     # BrowserStack parallel execution script
├── requirements.txt        # Project dependencies
├── README.md               # Project documentation
├── .gitignore              # Git ignore rules
└── .env                    # Environment variables (NOT committed)
⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone [https://github.com/your-username/browserstack-assignment.git](https://github.com/raikwarsagar2004-lab/Browser-Stack-Assessment)
cd browserstack-assignment
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Configure Environment Variables

Create a .env file in the project root directory:

BROWSERSTACK_USERNAME=your_browserstack_username
BROWSERSTACK_ACCESS_KEY=your_browserstack_access_key

⚠️ The .env file is excluded from version control for security purposes.

▶️ Local Execution

Run the main script locally to validate scraping and processing:

python main.py
This script will:

Verify that the website language is Spanish

Scrape the first 5 opinion articles

Extract article content and images

Translate titles into English

Perform repeated-word frequency analysis

🌐 BrowserStack Execution (Parallel Testing)

The solution runs on BrowserStack using 5 parallel sessions to validate cross-browser compatibility.

Browsers Tested

Chrome – Windows 11

Firefox – Windows 11

Edge – Windows 11

Safari – macOS Ventura

Chrome – Android (Samsung Galaxy S23)

Run on BrowserStack
python browserstack_run.py
Expected Output

5 live sessions visible in the BrowserStack dashboard

Console logs confirming execution on each platform

🔐 Security Considerations

BrowserStack credentials are stored using environment variables

No secrets are hard-coded in the repository

.env file is excluded via .gitignore

🧠 Key Highlights

Handles dynamic DOM content and multiple article layouts

Extracts paragraph text, standfirsts, and image captions

Deduplicates content while preserving reading order

Uses Selenium 4–compatible BrowserStack configuration

Demonstrates parallel execution across desktop and mobile browsers

✅ Assignment Completion

This implementation fulfills all requirements specified in the Round 2 – Technical Assignment, including:

✔ Web scraping
✔ API-based translation
✔ Text analysis
✔ Cross-browser parallel execution on BrowserStack
