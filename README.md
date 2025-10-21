# Real Estate Insights and Price Prediction Portal

This repository contains an advanced analytics platform for real estate insights and property price prediction using machine learning.

---

## Overview of the Website

The portal empowers users to:

- **Predict property prices** using state-of-the-art machine learning techniques.
- **Explore sector analytics** via interactive maps, pie charts, and various comparison plots.
- **Discover recommended apartments** based on location and important features.
- **Analyze trends** and compare features across different property types for smarter real estate decisions.

Our platform aims to provide buyers and sellers with reliable predictions, intelligent recommendations, and rich visualizations.

---

## Homepage

![Homepage Screenshot](README_images/home.png)

---

## Features Wordcloud

Visualizes important and popular features found in property listings to aid in feature importance analysis.

![Features Wordcloud](README_images/wordcloud.png)

---

## Price Prediction Example

Enter property details to view the predicted price range. Example output:

| property_type | sector | bedRoom | bathroom | balcony | agePossession | built_up_area |
|---------------|--------|---------|----------|---------|---------------|---------------|
| ...           | ...    | ...     | ...      | ...     | ...           | ...           |

The price of the flat is between **0.27 Cr and 0.71 Cr**.

![Price Prediction Output](README_images/price_prediction.png)

---

## Input Form Example

Enter your property parameters to get predictions (Property Type, Sector, Bedrooms, Bathrooms, etc).

![Input Form](README_images/input_form.png)

---

## Analytics

Explore price per square foot by location on the interactive geomap:

![Sector Price per Sqft Geomap](README_images/geomap.png)

---

## Area vs Price Scatter Plot

Visualize how built-up area relates to price for selected property types:

![Area vs Price](README_images/area_vs_price.png)

---

## BHK Pie Chart

See the distribution of BHK (bedroom) counts across sectors:

![BHK Pie Chart](README_images/bhk_pie.png)

---

## BHK Price Comparison

Boxplots comparing prices by number of bedrooms:

![BHK Price Comparison](README_images/bhk_price_comparison.png)

---

## Apartment Location & Radius Search

Find all apartments within a given radius of a selected location:

![Location and Radius Search](README_images/location_radius.png)

---

## Recommend Apartments

See top similar apartments based on a chosen reference property and similarity score:

| PropertyName            | SimilarityScore |
|-------------------------|----------------:|
| Ireo Victory Valley     |         0.8285  |
| Whiteland The Aspen     |         0.8204  |
| Adani M2K Oyster Grande |         0.816   |
| Pioneer Araya           |         0.791   |
| La Lagune               |         0.7877  |

![Recommend Apartments](README_images/recommend_apartments.png)

---

## How to Run This Application on AWS EC2

Deploy and run the Streamlit application on an AWS EC2 instance with these steps:

1. **Connect to Your EC2 Instance**
    ```
    ssh -i "C:\Users\91701\Downloads\streamlit_real_estate_app.pem" ubuntu@16.170.141.95
    ```

2. **Update and Upgrade Ubuntu Packages**
    ```
    sudo apt update && sudo apt upgrade -y
    ```

3. **Install Python and Pip**
    ```
    sudo apt install python3 python3-pip -y
    ```

4. **Install Streamlit**
    ```
    pip install streamlit --break-system-packages
    ```

5. **Install Required Python Packages**
    ```
    pip install -r requirements.txt --break-system-packages
    ```

6. **Add Python Binaries to PATH**
    ```
    export PATH=$PATH:/home/ubuntu/.local/bin
    ```

7. **Run the Streamlit App**
    ```
    streamlit run Home.py
    ```

Visit `http://<your-ec2-ip>:8501` in your browser to access the application.

---
