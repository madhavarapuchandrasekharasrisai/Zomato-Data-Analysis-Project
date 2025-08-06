# 📊 Zomato Data Analysis with Power BI

![Dashboard Preview](images/dashboard_preview.png)

An interactive Power BI dashboard that analyzes restaurant data from Zomato to uncover insights about customer behavior, cuisine popularity, pricing trends, and restaurant ratings across cities and countries.

---

## 🧰 Tools & Technologies

- **Power BI**
- **Excel**
- **Python (Pandas, NumPy)** – for data cleaning and transformation
- **DAX** – for calculated metrics and dynamic filters
- **Zomato Dataset** – from Kaggle or public sources

---

## 📸 Dashboard Snapshots

### 🍽️ Cuisine Popularity & Ratings

![Cuisine Insights](images/cuisine_insights.png)

---

### 🌍 Geographic Distribution of Restaurants

![Geo Map](images/geo_map.png)

---

### 💰 Cost for Two vs. Rating Comparison

![Cost Ratings](images/cost_ratings.png)

---

## 📌 Features

- ✅ Interactive filters: Country, City, Cuisine, Rating
- ✅ Cuisine-wise average rating and popularity charts
- ✅ Price comparison across different locations
- ✅ Geographic mapping of restaurant distribution
- ✅ DAX-based KPIs and calculated metrics
- ✅ Drill-through and tooltip insights
- ✅ Responsive and interactive dashboard layout

---

## 📁 Folder Structure

Zomato-Data-Analysis/
├── Zomato Project.pbit # Power BI Template File
├── README.md # This file
├── cleaned_zomato_data.csv # Cleaned dataset (optional)
└── images/
├── dashboard_preview.png
├── cuisine_insights.png
├── geo_map.png
└── cost_ratings.png

yaml
Copy
Edit

---

## 🧹 Data Cleaning Process

- Removed null, duplicate, and irrelevant records
- Standardized cuisine names and categorical fields
- Filtered dataset for selected cities/countries
- Converted columns like `cost_for_two` and `rating` to numeric
- Removed restaurants with zero reviews or missing data

---

## 📈 Example DAX Measures

```DAX
Average Rating = AVERAGE(Zomato[rating])

Total Restaurants = COUNT(Zomato[restaurant_id])

Cost Category = 
    SWITCH(TRUE(),
        Zomato[cost_for_two] <= 500, "Budget",
        Zomato[cost_for_two] <= 1500, "Mid-range",
        "Luxury"
    )
🔍 Insights Uncovered
Indian, North Indian, and Chinese are the top cuisines across major cities.

High ratings are not always tied to expensive restaurants.

Cities like Bangalore, Delhi, and Mumbai have a high concentration of top-rated places.

Some budget restaurants consistently receive better ratings than luxury ones.

The dataset reveals strong geographic and cultural patterns in food preferences.

🚀 How to Run the Project
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/zomato-data-analysis.git
Open the Zomato Project.pbit file using Power BI Desktop.

Load the provided cleaned_zomato_data.csv or connect to the dataset as needed.

Interact with the dashboard by using the filters and exploring various visuals.

🧠 What I Learned
Building visually appealing and interactive dashboards in Power BI

Cleaning and transforming real-world datasets using Python and Excel

Writing efficient and reusable DAX formulas

Using storytelling and data visualization techniques

Applying analytical thinking to draw business insights from data

📬 Contact
📧 your.email@example.com
🔗 LinkedIn
🔗 GitHub

📝 Note: Replace all placeholders like yourusername, email, and image paths with your actual project information before publishing on GitHub.

yaml
Copy
Edit

---

### 📝 Final Checklist for You:
- [ ] Replace `yourusername` in links.
- [ ] Replace `your.email@example.com`.
- [ ] Add your actual images to the `images/` folder.
- [ ] Rename image files if needed.
- [ ] Test the Markdown on GitHub for formatting.

Would you like help generating placeholder images or optimizing your screenshots before uploading the
