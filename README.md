# 🛒 Order-to-Cash (O2C) Process Analysis – E-Commerce Project

## 📌 Objective
This project analyzes the **Order-to-Cash (O2C)** process of an e-commerce business using real-world transactional data. The goal is to identify inefficiencies, detect bottlenecks, evaluate customer experience impact, and suggest actionable process improvements. The outcome is a **digital twin of the business process** that offers data-driven recommendations.

---

## 🔁 What is the Order-to-Cash (O2C) Process?

The O2C process encompasses all activities from a customer's order to payment and feedback. Key stages include:
1. **Order Placement**
2. **Order Approval**
3. **Order Invoicing & Payment**
4. **Order Picking & Shipping**
5. **Order Delivery**
6. **Customer Review / Feedback**

---

## 📊 Key Metrics by Phase

### 🟠 Order Processing
| Metric             | Description                                  |
|--------------------|----------------------------------------------|
| `approval_time`    | Time between order placement and approval    |
| `cancellation_rate`| % of canceled orders                         |

### 🔵 Shipping & Fulfillment
| Metric                  | Description                                           |
|-------------------------|-------------------------------------------------------|
| `shipping_time`         | Time from approval to shipment                        |
| `fulfillment_time`      | Total time from order to delivery                     |
| `on_time_delivery_rate` | % of orders delivered on or before promised date      |
| `delivery_delay_days`   | Days late for delayed deliveries                      |

### 🟢 Customer Feedback
| Metric                      | Description                                         |
|-----------------------------|-----------------------------------------------------|
| `avg_review_score`          | Average customer rating (1–5)                      |
| `review_score_by_delay`     | Reviews segmented by delivery timeliness           |
| `review_score_by_category`  | Reviews segmented by product or seller             |

### 💳 Payment & Value
| Metric                 | Description                                    |
|------------------------|------------------------------------------------|
| `avg_order_value`      | Average revenue per order                      |
| `avg_basket_size`      | Average number of items per order              |
| `payment_method_usage` | Payment behavior: Credit, UPI, Wallet, etc.    |

---

## 🧠 Why These Metrics Matter

- **📉 Bottleneck Detection**: Identify slow steps (e.g. long approval or shipping times)
- **⏱️ Operational Monitoring**: Assess if steps meet service expectations
- **😠 CX Impact**: Link delivery issues to bad reviews and churn
- **💰 Value Focus**: Prioritize high-value orders to reduce loss
- **🧩 Root Cause Analysis**: Slice metrics by category, region, seller to localize problems

---

## ✅ Project Structure

```bash
📁 O2C-Process-Analysis
├── 📁 sql_scripts/              # SQL scripts to create and populate tables in MS SQL Server
├── 📁 notebooks/                # Jupyter Notebooks (EDA, metrics, and insights)
├── 📁 dashboards/               # Power BI dashboard files connected to SQL Server
├── 📁 visuals/                  # Exported charts and graphs from EDA (Matplotlib/Seaborn)
├── 📁 data_sources/             # Original CSV files used to populate SQL database
├── 📄 README.md                 # Project documentation (this file)
└── 📄 requirements.txt          # Python libraries (e.g., pymysql, pandas, seaborn)

