# Brazilian E-Commerce Analytics Dashboard

An end-to-end Power BI dashboard analyzing 100k+ real orders from the Olist Brazilian E-Commerce dataset (Kaggle) — covering revenue trends, delivery performance, customer behavior, and seller/category analysis.

## 📥 Download the Dashboard
[Click here to download the full .pbix file (Google Drive)](https://drive.google.com/file/d/17QG9y3tIBjghYLzAzrEhmifFjE96xr-0/view?usp=sharing))

## 📊 Dashboard Pages
1. **Business Overview** — revenue growth, top categories, delivery & satisfaction snapshot
2. **Delivery Performance** — late delivery rates by state, delivery-timing vs. review score correlation
3. **Customer & Payments** — repeat customer rate, installment payment behavior, dynamic KPI selector
4. **Sellers & Categories** — seller ranking within category, freight cost efficiency

## 🔑 Key Findings
- Late deliveries correlate strongly with lower review scores (4.3 early vs 2.3 late average rating)
- Installment-payment orders average 73% higher value than single-payment orders
- Freight cost for bulky categories (furniture, home goods) can exceed 50% of product price

## 🛠️ Technical Highlights
- Custom star-schema data model built from 9 raw relational tables
- Role-playing date dimension using `USERELATIONSHIP`
- Dynamic Top-5 + "Others" grouping via `RANKX` and calculated tables
- Context transition handling across disconnected tables (payments ↔ order items)
- Fully dynamic KPI selector using `SWITCH` + `SELECTEDVALUE` on a disconnected table

## 📈 Data Source
[Olist Brazilian E-Commerce Public Dataset (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
