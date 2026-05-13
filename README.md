Smart Purchasing & Inventory Intelligence ToolWhy I Built This?In the world of supply chain, timing is everything



For a company importing goods from both the EU (30-day lead time) and China (90-day lead time), manual tracking is a recipe for disaster
 Ordering too early ties up valuable capital, while ordering too late leads to empty shelves and lost sales
 
 I developed this tool to bridge that gap. It isn’t just a collection of formulas it’s a Decision-Support System designed to give Supply Chain Managers instant, actionable insights. By automating the "Purchasing Meeting" preparation, it shifts the focus from "calculating numbers" to "making strategic moves
 
  Key FeaturesLive Inventory Health: No more digging through spreadsheets. The tool instantly flags every SKU as Order Now (Danger), Monitor (Warning), or OK (Safe).Lead Time Intelligence: It dynamically adjusts safety nets based on supplier location, ensuring that a 90-day transit from China doesn't catch the warehouse off-guard.ABC Financial Prioritization: Using the Pareto Principle, it identifies "Class A" items—the critical products that drive the majority of COGS spend—so you can prioritize high-value shipments.Scientific Order Quantities: Eliminates guesswork by calculating a Suggested Order Quantity that balances holding costs with service levels
  
  
The Logic Behind the ScenesTo ensure reliability, the tool implements industry-standard supply chain methodologies:
 Safety StockDesigned to absorb demand volatility and prevent stockouts
  
  
 Safety\ Stock = (Max\ Daily\ Sales - Avg\ Daily\ Sales) \times Lead\ Time
 
Reorder Point (ROP)The "Early Warning System" that triggers a new purchase order



ROP = (Avg\ Daily\ Sales \times Lead\ Time) + Safety\ Stock
 ABC ClassificationSegmenting inventory based on total investment:Class
 A: Top 70% of total spend (High Priority).Class
 B: Next 20% of spend (Medium Priority).Class
 C: Remaining 10% of spend (Low Priority). Project StructureInventory_Analysis.ipynb: The core analytical engine, featuring data cleaning, grouping, and logic implementation in Python
 Purchase_Order_Report.xlsx: The final output—a clean, management-ready report designed for immediate decision-making.inventory_dashboard.png: A high-level visual summary of warehouse health and spend distribution.supply_chain_dataset.csv: The historical sales and inventory data that powers the model
