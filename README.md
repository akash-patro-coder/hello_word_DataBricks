# hello_word_DataBricks
The "hello world" notebook introduces basic Databricks operations.  
The "basic pipeline" notebook demonstrates data processing across bronze, silver, and gold layers in a Delta Lake architecture.


┌─────────────┐
│   Bronze    │  Raw CSV ingestion                                                                                                                                                                       
│ (Raw Data)  │  → ecommerce_orders.csv                                                                                                                                                                  
└─────┬───────┘                                                                                                                                                                                          
      │                                                                                                                                                                                                  
      ▼
┌─────────────┐
│   Silver    │  Cleaned & Validated
│ (Delta)     │  → price > 0, qty > 0, delivered only
└─────┬───────┘
      │
      ▼
┌─────────────┐
│    Gold     │  Aggregated & KPIs
│ (Delta)     │  → revenue, orders, avg price
└─────────────┘
