# E-Commerce Customer Segmentation & Power BI Dashboard

This project performs a complete customer segmentation pipeline using the Online Retail dataset, followed by a Power BI dashboard for business insights.

It includes data cleaning, RFM analysis, behavioral metrics, clustering, persona creation, and marketing strategy recommendations.

---

## 📸 Dashboard Preview


### Home Page
![Home Page](https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail/raw/main/Screenshots/Screenshot%202025-11-08%20161256.png)

### Customer Overview
![Customer Overview](https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail/blob/main/Screenshots/Screenshot%202025-11-08%20161308.png)

### Customer Behavior
![Customer Behavior](https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail/blob/main/Screenshots/Screenshot%202025-11-08%20161319.png)

### Segment Profiles
![Segment Profiles](https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail/blob/main/Screenshots/Screenshot%202025-11-08%20161329.png)

### Revenue & Trends
![Revenue & Trends](https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail/blob/main/Screenshots/Screenshot%202025-11-08%20161343.png)

---

## 📁 Project Structure

```
customer_segmentation/
├── customer_segmentation.ipynb #  notebook
├── OnlineRetail.xlsx # Original dataset
├── Customer_Segmentation_Results.xlsx # Final segmentation output
│ ├── Customer_Features
│ ├── Segment_Profile
│ └── Personas
├── images/ # Dashboard screenshots
└── README.md # Documentation

```

---

## 🚀 Project Workflow

### 1. Data Cleaning  
Performed in **customer_segmentation.ipynb**:

- Removed cancelled orders  
- Removed negative prices/quantities  
- Removed missing CustomerIDs  
- Converted `InvoiceDate`  
- Created `TotalPrice`  
- Removed extreme outliers  

---

### 2. Feature Engineering

#### **RFM Metrics**
- Recency  
- Frequency  
- Monetary  

#### **Behavioral Metrics**
- Avg Basket Size  
- Avg Order Value  
- Number of Unique Products  
- Customer Lifetime  
- Order Frequency  


---

### 3. Customer Segmentation (K-Means)

Steps:

- Standardized features  
- Tested **K = 3 to K = 6**  
- Identified outliers  
- Selected optimal clusters  
- Visualized clusters using **PCA**  

📊 *Example PCA plot placeholder*

---

### 4. Segment Profiling

Each cluster analyzed based on:

- Recency  
- Frequency  
- Monetary  
- Behavioral metrics  
- Revenue contribution  


---

### 5. Persona Creation

Segments translated into simple business-friendly personas:

```

| Segment | Persona Name        | Description                              |
|--------|----------------------|-------------------------------------------|
| 0      | VIP Customers        | High-value, frequent buyers               |
| 1      | New/Active Customers | Recently engaged, strong growth potential |
| 2      | Other Customers      | Occasional but steady buyers              |
| 3      | At-Risk Customers    | Long time since last purchase             |
| 4      | Outliers             | Extreme value customers                   |

```
---

## ▶️ How to Run the Project

### **1️. Clone the repository**
```bash
git clone https://github.com/AkshayShetty7/Customer-Segmentation-Personalized-Marketing-in-Retail.git
cd Customer-Segmentation-Personalized-Marketing-in-Retail

```

### **2️. Install required Python libraries
```bash
pip install -r requirements.txt
```

### **3️. Open and run the Jupyter Notebook
```bash
jupyter notebook
```
Then open 
```bash
customer_segmentation.ipynb
```
Then run all cells 

Outputs are saved to
```bash
Customer_Segmentation_Results.xlsx
```

### **4️. Open the Power BI Dashboard**

1. Open **Power BI Desktop**
2. Load the **OnlineRetail Dashboard.pbix** file
3. Refresh the data source to pull updated segmentation results
4. Explore the dashboard pages:
   - **Home**
   - **Customer Overview**
   - **Customer Behavior**
   - **Segment Profiles**
   - **Revenue Trends**






