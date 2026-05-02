# 🥛 Nestlé Agri-Logistics Optimizer 
**Enterprise Supply Chain & Routing Proof of Concept**

## 📌 Overview
This project is a functional, interactive web application designed to optimize milk collection routes for Nestlé's Agri Services. Built over a 24-hour sprint, the dashboard calculates the most cost-effective and time-efficient paths for delivery trucks navigating between regional farms and centralized factory hubs. 

By prioritizing mathematical routing algorithms over expensive third-party APIs, this tool demonstrates how software engineering can directly reduce operational overhead in FMCG logistics.

## 🚀 Key Features
* **Dynamic Route Calculation:** Uses a Greedy Nearest-Neighbor algorithm to solve a localized Traveling Salesperson Problem (TSP) for fleet routing.
* **Real-World GPS Math:** Implements the **Haversine Formula** to calculate actual Earth-surface kilometers between latitude/longitude coordinates, rather than flat Euclidean lines.
* **Live Financial Metrics:** Instantly calculates Estimated Driving Time and Total Fuel Cost based on adjustable parameters (truck capacity, average speed, live diesel prices).
* **Interactive Cartography:** Dispatchers can click directly on the interactive Folium map to add new collection centers on the fly, triggering real-time route recalculation.
* **Exportable Manifests:** Includes a dedicated export tab to download high-resolution route maps and printable CSV driver manifests.

## 💻 Technical Architecture
* **Frontend/Framework:** Streamlit (Python)
* **Data Processing:** Pandas, NumPy
* **Geospatial Visualization:** Folium, Plotly Express, Streamlit-Folium
* **Core Logic:** Python `math` library for geospatial distance calculations.

## 📈 Business Value Impact
1. **Zero-Cost Operation:** Hardcoding the Haversine formula eliminates the need for paid routing services (like Google Maps API), resulting in $0 API overhead for the enterprise.
2. **Fuel Optimization:** Minimizes redundant driving miles, directly reducing fuel expenditure and carbon footprint.
3. **Agile Logistics:** Allows supply chain managers to simulate disruptions or new farm acquisitions instantly.

## ⚙️ How to Run Locally
1. Clone this repository to your local machine.
2. Install the required dependencies:
   ```bash
   pip install streamlit pandas numpy folium streamlit-folium plotly # Nestle-Agri-Logistics-Optimizer
