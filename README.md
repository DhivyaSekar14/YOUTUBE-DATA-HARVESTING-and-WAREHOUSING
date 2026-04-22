# Youtube-Data-Harvesting-and-Warehousing
YouTube Data Harvesting and Warehousing is a Streamlit app that fetches channel data via YouTube API. It uses MongoDB for unstructured storage and migrates data to MySQL for structured warehousing. Features include automated table creation, multi-channel data extraction, and an Insights dashboard for advanced SQL querying.
##  Features
- **Data Extraction:** Fetch channel, video, and comment details using YouTube API.
- **Data Lake:** Store raw JSON-like data in MongoDB.
- **Data Warehouse:** Transform and migrate data into a structured MySQL database.
- **SQL Analytics:** 10+ pre-defined queries to gain insights into video performance, engagement, and channel growth.

##  Tech Stack
- **Frontend:** Streamlit
- **API:** Google API Client (YouTube V3)
- **Databases:** MongoDB (NoSQL), MySQL (SQL)
- **Data Processing:** Pandas, Regex, Dateutil

##  Configuration
1. **API Key:** Obtain a YouTube Data API key from Google Cloud Console.
2. **MongoDB:** Ensure MongoDB is running locally at `mongodb://localhost:27017/`.
3. **MySQL:** Set up a local instance. Update the credentials in the code:
   - User: `root`
   - Password: `your_password`
   - Database: `youtube_data`

##  How to Run
pip install -r requirements.txt
streamlit run youtube_app.py
