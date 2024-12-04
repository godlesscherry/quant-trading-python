# Iceberg Order Detection Notebook

This project provides a Python-based implementation to detect iceberg orders in trading data using order book analysis. The notebook demonstrates how to identify hidden large orders (iceberg orders) by analyzing bid-ask imbalances and visualizing potential signals.

---

## Explanation of the Notebook

### **Order Book Data**
The sample data includes:
- `price`: The price levels in the order book.
- `bid_size`: Total volume of bids (buy orders) at each price level.
- `ask_size`: Total volume of asks (sell orders) at each price level.
- `bid_orders`: Number of bid orders at each price level.
- `ask_orders`: Number of ask orders at each price level.

---

### **Bid-Ask Imbalance**
**Imbalance** is a measure of the difference between the bid and ask sizes relative to the total volume. It is calculated as:
**Imbalance Formula**:
```
imbalance = (bid size - ask size) / (bid size + ask size)
```


---

### **Iceberg Detection Criteria**
To detect potential iceberg orders, the following conditions are used:
1. **High Bid-Ask Imbalance**: 
   - Imbalance greater than `0.6` indicates a significantly higher demand on the bid side.
2. **Low Number of Bid Orders**:
   - A small number of bid orders (`bid_orders < 10`) suggests the presence of large hidden orders.

---

### **Visualization**
- A bar plot visualizes the bid-ask imbalance for each price level.
- Red markers highlight detected iceberg orders that meet the criteria.

---

### **Output**
The output includes a table showing:
- Prices where iceberg orders are detected.
- Details like bid size, ask size, and the calculated imbalance.

---

## **Why Are Iceberg Orders Important?**

### **What Are Iceberg Orders?**
Iceberg orders are large hidden orders in the market, where only a fraction of the total order size is visible at a time. The hidden part is revealed gradually as the visible part is filled.

### **Why Detect Iceberg Orders?**
1. **Market Insights**:
   - Identifying iceberg orders can reveal significant buying or selling pressure in the market.
   - Helps traders anticipate large market moves.

2. **Execution Strategies**:
   - Traders can adjust their strategies to avoid getting caught in the wrong direction when iceberg orders are present.

3. **Competitive Advantage**:
   - Spotting hidden liquidity gives a trader an edge in predicting price movements.

4. **Risk Management**:
   - Recognizing iceberg orders helps avoid liquidity traps and unexpected volatility.

---
