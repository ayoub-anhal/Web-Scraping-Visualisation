# 🍽️ Bangkok Restaurants Data Explorer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-4.9%2B-green)
![Tableau](https://img.shields.io/badge/Tableau-Public-orange)

A comprehensive data collection and visualization project extracting insights from Bangkok's top restaurants on TripAdvisor.

![Project Architecture](https://github.com/ayoub-anhal/Web-Scraping-Visualisation/blob/main/rapport/Diagramme.png)

##  Table of Contents
- [Project Overview](#-project-overview)
- [Features](#-features)
- [Repository Structure](#-repository-structure)
- [Technologies](#-technologies)
- [Installation & Setup](#-installation--setup)
- [Usage](#-usage)
- [Data Collection Process](#-data-collection-process)
- [Visualization](#-visualization)
- [License](#-license)
- [Contributors](#-contributors)

##  Project Overview

This project combines web scraping techniques with data visualization to analyze Bangkok's restaurant scene. By extracting data from TripAdvisor's Bangkok restaurant listings and visualizing it through an interactive Tableau dashboard, we enable comprehensive analysis of restaurant trends, ratings, cuisines, and customer sentiments.

##  Features

- **Comprehensive Data Collection**: Extraction of detailed information from Bangkok's top 500 restaurants
- **Rich Review Analysis**: Collection and analysis of customer reviews for sentiment and keyword trends
- **Interactive Visualization**: Tableau Public dashboard providing multiple views of the restaurant landscape
- **Scalable Architecture**: Designed for potential expansion to other cities or platforms

##  Repository Structure

```
├── TripAdvisor.ipynb     # Main Jupyter notebook for web scraping
├── restaurants.json      # Structured data of restaurant details
├── all_reviews.json      # Comprehensive collection of restaurant reviews
├── rapport/              # Project documentation
│   └── Diagramme.png     # Project architecture diagram
└── README.md             # Project documentation (you are here)
```

##  Technologies

- **Web Scraping**:
  - Python 3.8+
  - BeautifulSoup4
  - Oxylabs (Web Scraping API)
  - Jupyter Notebook

- **Data Processing**:
  - Pandas
  - JSON

- **Visualization**:
  - Tableau Public

##  Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/ayoub-anhal/Web-Scraping-Visualisation.git
   cd Web-Scraping-Visualisation
   ```

2. Set up Python environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Configure Oxylabs credentials in the notebook:
   ```python
   # Set your Oxylabs credentials in the notebook
   username = "YOUR_USERNAME"
   password = "YOUR_PASSWORD"
   ```

##  Usage

1. **Data Collection**:
   - Open and run the `TripAdvisor.ipynb` notebook:
   ```bash
   jupyter notebook TripAdvisor.ipynb
   ```
   - Follow the notebook instructions to scrape restaurant data

2. **Data Exploration**:
   - Examine the generated `restaurants.json` and `all_reviews.json` files
   - Use pandas to perform preliminary analysis

3. **Visualization**:
   - Access the interactive dashboard:
   [Bangkok Restaurants Dashboard](https://public.tableau.com/views/DASHBangkok/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

##  Data Collection Process

The data collection process involves:

1. **Initial Scraping**: Accessing TripAdvisor's Bangkok restaurant listings page
   ```
   https://www.tripadvisor.com/Restaurants-g293916-Bangkok.html
   ```

2. **Restaurant Data Extraction**: For each restaurant, we collect:
   - Name and URL
   - Rating (1-5 stars)
   - Number of reviews
   - Price range
   - Cuisine types
   - Location

3. **Review Collection**: For each restaurant, we scrape:
   - Review text
   - Rating
   - Date of visit
   - User information

4. **Data Storage**: All information is structured and stored in JSON format.

##  Visualization

The Tableau dashboard provides multiple views:

- Restaurant distribution by location
- Rating analysis
- Price range distribution
- Cuisine popularity
- Sentiment analysis of reviews
- Keyword frequency in positive and negative reviews

**Access the dashboard here**: [Bangkok Restaurants Tableau Dashboard](https://public.tableau.com/views/DASHBangkok/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

##  License

This project is licensed under the MIT License - see the LICENSE file for details.

##  Contributors

- [Ayoub Anhal](https://github.com/ayoub-anhal)

---

*Note: This project is for educational purposes. Please respect TripAdvisor's terms of service when using their data.*
