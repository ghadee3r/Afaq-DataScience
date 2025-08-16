# Afaq – Unveiling Saudi Arabia’s Hidden Gems Through Data  

Afaq (آفاق) is a data science project developed for **IT362 – Data Science**.  
The project explores underappreciated tourist destinations in Saudi Arabia by analyzing public photo data from Flickr. Using machine learning and data analytics, it identifies hidden gems, seasonal trends, and the visual features that make destinations appealing.  

---

## Project Overview  

Saudi Arabia has a rich variety of natural landscapes, cultural sites, and historical attractions. Many of these remain overlooked in tourism promotion. This project leverages **Flickr image data and metadata** to uncover which destinations attract the most engagement and how factors like season, time of day, region, and visual elements influence popularity.  

---

## Objectives  

- Identify attractions in Saudi Arabia that deserve more attention based on photo engagement.  
- Analyze how destination popularity changes across seasons.  
- Determine which times of day attract the most photo interactions.  
- Explore which visual elements (e.g., trees, buildings, mountains, water) appear most in popular photos.  
- Compare engagement across different regions to highlight underpromoted areas.  

---

## Data & Methods  

- **Data Source:** Flickr API (photo metadata, favorites, comments, views).  
- **Feature Extraction:**  
  - *CLIP (OpenAI)* – classified visual elements.  
  - *OpenCV* – identified day/night from brightness.  
  - *Hugging Face Transformers* – sentiment analysis of comments.  
- **Data Transformation:** Structured 199 public photos into a dataset of 33 features.  
- **Analysis:** Exploratory data analysis, correlations, engagement by region/season/time.  
- **Modeling:** Regression models to predict a **Popularity Score**.  
  - Linear Regression (baseline)  
  - Random Forest Regressor (best performing, R² = 0.93)  
  - Support Vector Regressor (underperformed)  

---

## Key Findings  

- **Regions:** Eastern and Northern regions had the highest tourism appeal; the Southern region was consistently underrepresented and under-engaged.  
- **Seasons:** Autumn showed peak engagement across multiple regions.  
- **Time of Day:** Daytime photos had higher popularity overall, except in the West, where nighttime photos performed better.  
- **Visual Elements:** Mountains, coastal landscapes, and historical sites stood out as most appealing.  
- **Model Results:** Random Forest captured engagement patterns best, explaining 93% of variance.  

---

## Challenges  

- Limited and incomplete metadata from Flickr.  
- Seasonal bias in photo availability.  
- Time-consuming image processing.  
- Some regions (e.g., South) underrepresented in the dataset.  

---

## Future Work  

- Expand data sources (Instagram, TripAdvisor, Google Maps).  
- Improve image classification accuracy by fine-tuning CLIP for tourism contexts.  
- Use temporal models (LSTM, ARIMA) for seasonality analysis.  
- Collaborate with tourism authorities to promote low-engagement regions.  

---

## Contributors  

- Ghadeer Alnuwaysir – 444200420  
- Maha Alruwais – 444200749  
- Norah Almadhi – 444200890  
- Rana Albridi – 444201094  
- Lamees Alghamdi – 444201177  

**Supervisor:** Dr. Mashael Sultan Aldayel  

