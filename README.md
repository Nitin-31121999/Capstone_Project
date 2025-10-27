# Real Estate Insights and Price Prediction Portal

## Overview of the Website

The portal empowers users to:

- **Predict property prices** using state-of-the-art machine learning techniques.
- **Explore sector analytics** via interactive maps, pie charts, and various comparison plots.
- **Discover recommended apartments** based on location and important features.
- **Analyze trends** and compare features across different property types for smarter real estate decisions.

Our platform aims to provide buyers and sellers with reliable predictions, intelligent recommendations, and rich visualizations.

---


### Homepage

![Homepage Screenshot](https://github.com/Nitin-31121999/Capstone_Project/blob/44a00b579bcddd3100ebd9c960e3b96ddb8b734b/Screenshot%202025-10-21%20221953.png)

---

### Geospatial analysis

![Geospatial analysi](https://github.com/Nitin-31121999/Capstone_Project/blob/aed48f91258ecccb419214ff243823e9ab284536/Screenshot%202025-10-21%20222213.png)

---

### Input Form

![Input Form](https://github.com/Nitin-31121999/Capstone_Project/blob/3213b5111f5f7ce7a99d5eb9a4c084bea51ea9eb/Screenshot%202025-10-21%20222026.png)
---

### Price Prediction Example

| property_type | sector | bedRoom | bathroom | balcony | agePossession | built_up_area |
|---------------|--------|---------|----------|---------|---------------|---------------|
| ...           | ...    | ...     | ...      | ...     | ...           | ...           |

The price of the flat is between **0.27 Cr and 0.71 Cr**.

![Price Prediction Output](https://github.com/Nitin-31121999/Capstone_Project/blob/e04dfb49f780027a23b6d297c4541e3fadbe9b9a/Screenshot%202025-10-21%20222127.png)

---


### Features Wordcloud

![Features Wordcloud](https://github.com/Nitin-31121999/Capstone_Project/blob/48aba5f614e3c7a3e25bccfd98993bc8f11bec0e/Screenshot%202025-10-21%20222225.png)

---

### Area vs Price Scatter Plot

![Area vs Price](https://github.com/Nitin-31121999/Capstone_Project/blob/f9e6be5afdea75111c90c0f599f81762441da914/Screenshot%202025-10-21%20222235.png)

---

### BHK Pie Chart

![BHK Pie Chart](https://github.com/Nitin-31121999/Capstone_Project/blob/30a85521686712a8d7e3dd71fb342f71b565843c/Screenshot%202025-10-21%20222258.png)

---

### BHK Price Comparison

![BHK Price Comparison](https://github.com/Nitin-31121999/Capstone_Project/blob/f4f70f2e707050431b41efe05863099b51e3c787/Screenshot%202025-10-27%20102419.png)

---

### Apartment Location & Radius Search

![Location and Radius Search](https://github.com/Nitin-31121999/Capstone_Project/blob/5948bb54a86ea34dec1a45209cb634fbad491d36/Screenshot%202025-10-21%20222427.png)

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
