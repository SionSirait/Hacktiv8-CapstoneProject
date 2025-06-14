# 🏬 Singapore Shopping Mall Development Analysis

This project uses **geolocation data** and **clustering algorithms** to identify strategic zones in Singapore for future shopping mall development. It applies a **data science approach** to urban retail planning using Python and Foursquare API.

## 📌 Project Goals

- Identify areas in Singapore that are:
  - ✅ Underserved (ideal for development)
  - ⚠️ Moderately competitive
  - ❌ Oversaturated
- Provide decision-making support for developers, investors, and planners

## 🗂 Data Sources

- 📍 [Wikipedia – Places in Singapore](https://en.wikipedia.org/wiki/Category:Places_in_Singapore)  
- 📡 [Foursquare Places API](https://location.foursquare.com/places)

## ⚙️ Tools & Technologies

- **Python** (Jupyter Notebook via Google Colab)
  - `requests`, `BeautifulSoup` (web scraping)
  - `geopy`, `geocoder` (geolocation)
  - `pandas`, `numpy` (data wrangling)
  - `scikit-learn` (K-Means clustering)
  - `folium`, `matplotlib` (visualization)
- **GitHub** (project repository)
- **Power BI & Tableau** (dashboard prototyping – optional)

## 🧪 Methodology

1. **Extracted** 16 key locations from Wikipedia
2. **Geocoded** using `geopy` to get lat/lon
3. **Retrieved venue data** using Foursquare API (1 km radius, limit 50)
4. **Filtered** for “Shopping Mall” venues
5. **Calculated** mall frequency metric per area
6. **Clustered** areas using KMeans (k=3)
7. **Mapped** results to identify strategic retail zones

## 📊 Key Findings

| Cluster | Description                    | Example Areas                  | Recommendation         |
|---------|--------------------------------|--------------------------------|-------------------------|
| 1       | Underserved residential zones  | Punggol, Sembawang, Pasir Ris | ✅ Build here           |
| 0       | Moderately competitive         | Toa Payoh, Tampines, Serangoon| ⚠️ Build with USP       |
| 2       | Oversaturated central areas    | Orchard, Bugis, Marina Bay     | ❌ Avoid traditional malls |

## Author

**Sion Yehuda Radja Abednego**  
Business Management Graduate  
[LinkedIn](#) | [Email](mailto:sionyehuda05@gmail.com)

---

