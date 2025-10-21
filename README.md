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

## Screenshots

### Homepage

![Homepage Screenshot](<img width="1672" height="781" alt="Screenshot 2025-10-21 221953" src="https://github.com/user-attachments/assets/21216be4-8b0e-46c0-98cf-c8ad4def7001" />
)

---

### Geospatial analysis

![Geospatial analysi](<img width="727" height="809" alt="Screenshot 2025-10-21 222213" src="https://github.com/user-attachments/assets/7ba9134a-2b64-496c-b5c6-d1254143c38b" />
)

---

### Input Form

![Input Form](<img width="609" height="856" alt="Screenshot 2025-10-21 222108" src="https://github.com/user-attachments/assets/f60d3155-f4d8-449f-9bd4-a831d5a9a1f1" />
)

---

### Price Prediction Example

| property_type | sector | bedRoom | bathroom | balcony | agePossession | built_up_area |
|---------------|--------|---------|----------|---------|---------------|---------------|
| ...           | ...    | ...     | ...      | ...     | ...           | ...           |

The price of the flat is between **0.27 Cr and 0.71 Cr**.

![Price Prediction Output](<img width="557" height="124" alt="Screenshot 2025-10-21 222127" src="https://github.com/user-attachments/assets/3b9967ae-6ee6-4a96-8999-887a1f90c340" />
)

---


### Features Wordcloud

![Features Wordcloud](<img width="840" height="817" alt="Screenshot 2025-10-21 222225" src="https://github.com/user-attachments/assets/7e7dbee1-4f1a-457c-bcc1-8ec2bb44adf7" />
)

---

### Area vs Price Scatter Plot

![Area vs Price](<img width="844" height="608" alt="Screenshot 2025-10-21 222235" src="https://github.com/user-attachments/assets/d6330030-29c1-4faf-99e3-f8bdf87a5b33" />
)

---

### BHK Pie Chart

![BHK Pie Chart](<img width="859" height="620" alt="Screenshot 2025-10-21 222258" src="https://github.com/user-attachments/assets/8f771466-dd29-4d65-b8c9-0cdbd8aff26b" />
)

---

### BHK Price Comparison

![BHK Price Comparison](<img width="767" height="522" alt="Screenshot 2025-10-21 222316" src="https://github.com/user-attachments/assets/ddc49753-295b-4418-b105-0c560180ffe3" />
)

---

### Apartment Location & Radius Search

![Location and Radius Search](https://private-user-images.githubusercontent.com/177639605/503805242-a9b82cf4-6fa0-4920-a8fc-1f698557c022.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjEwNjg5MTgsIm5iZiI6MTc2MTA2ODYxOCwicGF0aCI6Ii8xNzc2Mzk2MDUvNTAzODA1MjQyLWE5YjgyY2Y0LTZmYTAtNDkyMC1hOGZjLTFmNjk4NTU3YzAyMi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDIxJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAyMVQxNzQzMzhaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03YzE4YzJiMmFjYzU2N2Q0ZjkzZGNmOTk4MTg2NjM1MzFmZWU4NTRjYzdjMmI0MjAyYjM0MTI2OTU5NGE5ZWY3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.8iG1GweQcOSEehGYEu6FHVWFcjdVo5NVTCSgO2cQEXo)

---

### Recommend Apartments

| PropertyName            | SimilarityScore |
|-------------------------|----------------:|
| Ireo Victory Valley     |         0.8285  |
| Whiteland The Aspen     |         0.8204  |
| Adani M2K Oyster Grande |         0.816   |
| Pioneer Araya           |         0.791   |
| La Lagune               |         0.7877  |


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
