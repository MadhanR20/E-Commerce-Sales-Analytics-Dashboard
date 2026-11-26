# 📊 Amazon Sales Analytics Dashboard

> An interactive Tableau dashboard visualizing Amazon India's sales data — uncovering sales patterns, category performance, geographic distribution, and customer behavior from **March to June 2022**.

![Dashboard Preview](docs/dashboard_preview.png)

---

## 🧩 Background

This dataset originates from **Amazon India's** e-commerce platform, recording all transaction activity over approximately 3 months. The data covers complete information ranging from product details (category, size, SKU), shipping status, delivery location, to transaction value — making it a rich source for end-to-end sales analysis.

This project aims to answer key business questions such as:
- Which product categories are the best sellers and generate the most revenue?
- Which provinces have the highest concentration of sales?
- How significant is the order cancellation rate and what is its impact?
- Does the B2B segment contribute meaningfully to total sales?

---

## 📂 Folder Structure

```
amazon-sales-analytics/
│
├── data/
│   └── raw/
│       └── amazon_sale_report.csv        ← original dataset (128K+ rows)
│
├── tableau/
│   └── Amazon_Sales_Analytics_Dashboard.twbx
│
├── docs/
│   └── dashboard_preview.png
│
└── README.md
```

---

## 📋 About the Dataset

| Attribute | Detail |
|-----------|--------|
| **Source** | Amazon India — Internal Sales Report |
| **Period** | March 31 – June 29, 2022 |
| **Total Transactions** | 128,975 rows |
| **Currency** | ₹ INR (Indian Rupee) |
| **Total Revenue** | ₹78,590,257 |
| **Total Units Sold** | 116,649 units |
| **Unique Products** | 7,190 SKUs |
| **Total Categories** | 9 categories |
| **Size Variations** | 11 sizes |

### Column Reference (23 Columns)

| Column | Description |
|--------|-------------|
| `Order ID` | Unique identifier for each transaction |
| `Date` | Date the order was placed |
| `Status` | Order status (Shipped, Cancelled, Returned, etc.) |
| `Fulfilment` | Fulfillment method (Amazon / Merchant) |
| `Sales Channel` | Sales platform (Amazon.in / Non-Amazon) |
| `ship-service-level` | Shipping service type (Expedited / Standard) |
| `Category` | Fashion product category |
| `Size` | Product size (XS, S, M, L, XL, XXL, 3XL, etc.) |
| `Qty` | Number of units ordered |
| `Amount` | Transaction value in INR |
| `ship-state` | Destination state/province |
| `B2B` | Whether the transaction is Business-to-Business |
| `Courier Status` | Courier delivery status |

### Product Categories

| Category | Description |
|----------|-------------|
| Set | Complete clothing sets |
| Kurta | Traditional Indian top wear |
| Western Dress | Western-style dresses |
| Top | Casual tops |
| Ethnic Dress | Traditional ethnic wear |
| Bottom | Trousers and skirts |
| Saree | Traditional Indian draped garment |
| Blouse | Formal/casual blouses |
| Dupatta | Traditional Indian scarf |

---

## 📊 Key Insights from the Dashboard

### 1. 📦 Shipping Status
The vast majority of orders were successfully processed. **94.21%** of orders have a *Shipped* status, while **5.79%** remain *Unshipped*. The cancellation rate stands at **4.39%** of total transactions — a figure worth monitoring as it directly impacts revenue and customer experience.

### 2. 🗺️ Geographic Distribution
Sales are concentrated in a few major Indian states. **Maharashtra** and **Karnataka** dominate sales volume, followed by **Uttar Pradesh**, **Tamil Nadu**, and **Telangana**. This indicates that urban markets in western and southern India represent the primary consumer base for Amazon India.

### 3. 👗 Category Performance
The **Set** and **Kurta** categories are the best performers both in unit volume and revenue. Traditional Indian ethnic fashion dominates transactions, reflecting strong local consumer preference for traditional clothing.

### 4. 📏 Size Distribution
**Medium (M)** and **Large (L)** are the most frequently ordered sizes, followed by **XL** and **XXL**. Extreme sizes such as 4XL, 5XL, and 6XL show very low volume — valuable information for inventory management and stock planning.

### 5. 🏢 B2B Segment
B2B transactions account for only **0.72%** of total orders — the overwhelming majority (99.28%) are direct-to-consumer (B2C) sales. This indicates that Amazon India's customer base is primarily composed of individual consumers rather than resellers or businesses.

### 6. 🛒 Sales Channel
**99.86%** of transactions originate from the Amazon.in platform, with Non-Amazon channels contributing only **0.14%**. This dominance reflects a highly centralized ecosystem with minimal off-platform activity.

### 7. 📈 Weekly Trend
Sales peaked during the **first week of May 2022**, followed by a gradual decline toward the end of June. This trend may indicate the influence of promotional events or seasonal shopping behavior specific to the Indian market.

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/elsaveroo/amazon-sales-analytics.git
   cd amazon-sales-analytics
   ```

2. Open the dashboard:
   - Download and install [Tableau Public](https://public.tableau.com/en-us/s/download) (free)
   - Open `tableau/Amazon_Sales_Analytics_Dashboard.twbx`
   - The dashboard is ready to use — data is already embedded inside the `.twbx` file

3. Available interactive filters:
   - **Category** — filter by product category
   - **Time period** — drill down by week

---

## 🛠️ Tools & Tech Stack

| Tool | Purpose |
|------|---------|
| **Tableau Public** | Data visualization & dashboard |
| **CSV** | Raw data format |
