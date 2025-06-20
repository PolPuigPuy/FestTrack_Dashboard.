# FestTrack_Dashboard.
A data analytics dashboard for the Cruïlla Festival 2024, combining social media sentiment, music platform metrics, and artist growth predictions.

This project presents an interactive dashboard that monitors and analyzes audience engagement around the Cruïlla Festival 2024. It integrates data from social media platforms (Twitter, Instagram, TikTok) and music services (Spotify, YouTube, Apple Music) to assess artist popularity, track sentiment trends, and evaluate the impact of the festival on the artists. Through visualizations, geolocation maps, and a machine learning model trained to predict artist growth, the dashboard offers organizers and stakeholders a complete picture of public perception and marketing effectiveness.

**How to make use of the device:**
To run the Cruïlla Festival dashboard, the only requirement is to have Python installed along with the necessary libraries listed in the requirements.txt file. To get started, the professor should first open a terminal in the project directory and run the following command to install all dependencies (if this doesn’t work we recommend manually installing them):
 -- pip install -r requirements.txt
Additionally, since the Instagram analysis uses spaCy for natural language processing in Spanish, it is necessary to download the es_core_news_sm language model with this command:
 -- python -m spacy download es_core_news_sm
Once all dependencies are installed, the dashboard can be launched by running:
 -- streamlit run app.py
This command will open a browser window showing the interactive dashboard, organized into multiple tabs that cover different data sources (Spotify, TikTok, Instagram, Twitter, YouTube, Apple) and analysis perspectives (sentiment, engagement, artist metrics, and prediction).
If any information displayed on the dashboard needs to be updated (for instance to compute the metrics for 2025), such as artist metrics, sentiment analysis, or predictions, you should consider the following.
To retrieve data we used Apify and Chartmetrics. Under the original_data folder we showcase what type of data we started with.
We then used the files in the prepare_data folder to preprocess the data and create some visualizations for the dashboard
Lastly the final data the dashboard needs is displayed in the clean_data repository, which should then be replaced by the data previously processed if you wanted to visualize next years’ dashboard.
Once updated, simply relaunch the app using the streamlit run app.py command. The dashboard will automatically reflect the new data without needing to modify the code.
