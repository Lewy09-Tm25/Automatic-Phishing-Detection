# Automatic Phishing Detection

This repository replicates and extends the work of Pandey and Mishra (2023) where they use the color pallette of a website in order to understand if a given website is phishing or not. Our extension to the work is we add NLP based features based on the URL and the actual text of the website. We achieve 84% accuracy using a random forest on our new feature set.

To use any of these files, please

pip install -r requirements.txt

The directory is as follows:
- /data contains links and scraped data used for the research
- /metrics contains the metrics from our run of the repo
- /models contains pickled models for future use
- /notebooks contains our EDA, model deep dives, and our attempt at direct replication of Pandey and Mishra (2023)
- web_scraping.py is the script which does its namesake. It uses selenium and does a bulk of the feature extraction
- preprocessing.py cleans the data and continues a bit of the feature extraction
- classical_trainer.py tunes and trains the classical ML models and stores their results in metrics/.
