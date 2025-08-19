# hello_word_DataBricks
The "hello world" notebook introduces basic Databricks operations.  
The "basic pipeline" notebook demonstrates data processing across bronze, silver, and gold layers in a Delta Lake architecture.


**Bronze (Raw Data)**
- Source: `ecommerce_orders.csv`

⬇️

**Silver (Delta)**
- Cleaned & Validated  
  - price > 0  
  - qty > 0  
  - delivered only  

⬇️

**Gold (Delta)**
- Aggregated & KPIs  
  - revenue  
  - orders  
  - avg price  

