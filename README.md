📩 SMS Spam Classification & Dataset Creation

🚀 Overview

This project presents an AI-driven pipeline for extracting, processing, and classifying SMS messages into spam and non-spam categories.
It integrates data engineering (XML parsing) with NLP-based classification to build a scalable and automated spam detection system.

⸻

❗ Problem Statement

With the exponential rise in mobile communication, SMS spam (phishing, scams, promotional messages) has become a major threat to users.
Manual filtering is inefficient, error-prone, and non-scalable.

👉 Goal: Design a system that can automatically classify SMS messages into meaningful spam categories using computational intelligence.

⸻

🎯 Objectives

* Extract SMS data from XML backup files
* Convert raw messages into structured datasets
* Automatically classify SMS into spam categories
* Reduce manual labeling effort
* Build a scalable and efficient classification pipeline

⸻

🧠 Methodology

🔹 1. SMS Data Parsing (XML → Structured Dataset)

* Extracted SMS messages from XML backup files
* Retrieved key fields:
    * Sender
    * Timestamp (converted to readable format)
    * Message body
    * Message type (Inbox, Sent, etc.)
* Cleaned and preprocessed data:
    * Handled missing/invalid timestamps
    * Removed encoding errors
* Generated structured dataset using Pandas DataFrame

⸻

🔹 2. SMS Classification System

Messages were classified into the following categories:

* Phishing
* Smishing
* Promotional
* Loan / Financial Scam
* Job Scam
* Crypto / Investment Scam
* No Spam

⸻

🔹 3. Model & Approach

* Utilized multiple pre-trained language models via API:
    * deepseek-v3
    * qwen-coder
    * gpt-oss models
* Implemented an ensemble strategy:
    * Majority voting
    * Confidence score aggregation
* Flagged low-confidence predictions for manual review

⸻

⚙️ Tech Stack

* Programming: Python
* Libraries: Pandas, XML Parsing
* Domain: Natural Language Processing (NLP)
* Models: Pre-trained LLMs (API-based)
* Data Format: XML → CSV

⸻

⚠️ Challenges Faced

* API rate limits restricted classification speed
* Variations in XML formats caused parsing issues
* Missing or inconsistent timestamps
* Large dataset size increased processing time
* Ambiguous SMS content reduced classification accuracy
* Class imbalance in spam vs non-spam data

⸻

📊 Key Outcomes

* Structured and cleaned SMS dataset (CSV format)
* Automated spam classification system
* Reduced manual labeling effort significantly
* Scalable pipeline for large SMS datasets

⸻

📌 Applications

* 📱 Mobile spam filtering systems
* 📡 Telecom fraud detection
* 🏢 Enterprise communication monitoring
* 🔍 NLP research on SMS datasets
* 💳 Financial fraud detection systems

⸻

🚧 Limitations

* Dependency on external APIs (rate limits)
* Batch processing (no real-time filtering)
* Performance affected by ambiguous messages
* XML format dependency
* Limited generalization to unseen formats/languages

⸻

💡 Why Automated Labeling?

* Manual labeling is time-consuming and inconsistent
* Large datasets make manual work impractical
* Automation ensures:
    * Speed ⚡
    * Accuracy 🎯
    * Scalability 📈

⸻

👥 Team Members

This project was developed as part of an academic group project:

* 22BCS098 – Rishabh Yadav
* 22BCS096 – Rachakonda Shrutik Sai
* 22BCS093 – Priyanshu Raj
* 22BDS021 – Gaikwad Aman Anand
* 22BCS113 – Shashank R Acharya

⸻

📂 Repository Structure

📦 sms-spam-classification
 ┣ 📂 data                # Raw & processed datasets
 ┣ 📂 src / notebooks     # Code files
 ┣ 📂 docs
 ┃   ┣ project_report.pdf
 ┃   ┣ presentation.pptx
 ┣ README.md

⸻

📚 References

* UCI SMS Spam Collection Dataset
* IEEE Research Papers on Spam Detection
* GeeksforGeeks Machine Learning Resources
* Research surveys on SMS spam classification

⸻

✅ Conclusion

This project demonstrates how raw SMS data can be transformed into structured datasets and classified using AI-driven techniques.
By combining data parsing, preprocessing, and ensemble classification, the system achieves a scalable and practical solution for SMS spam detection.

⸻

⭐ Future Improvements

* Real-time SMS classification system
* Fine-tuned transformer models (BERT-based)
* Improved dataset balancing techniques
* Deployment as a mobile or web application

