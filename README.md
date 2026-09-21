# Day 29: Product Basket Analysis

## Objective
Introduce association-style analysis to uncover purchasing patterns and find products frequently purchased together to inform cross-selling strategies.

## Technical Implementation
* **Tools Used:** Python (Pandas, NumPy, Itertools).
* **Methodology:** 
  * Aggregated a normalized transactional dataset by `OrderID` to reconstruct individual customer shopping baskets.
  * Generated unique product pair combinations utilizing `itertools.combinations`, ensuring data integrity by sorting items and explicitly excluding self-pairs.
  * Tabulated frequency counts across 500 simulated transactions to identify statistically significant co-purchasing behaviors.

## Key Insights & Recommendations
* **Top Product Pairs:** The analysis identified a **Webcam and Wireless Mouse** as the highest-frequency product combination, co-occurring in 102 distinct orders. Other high-frequency pairs included the Mechanical Keyboard and Webcam (95 occurrences).
* **Recommendations:** Based on these findings, the marketing team should configure the e-commerce platform's recommendation engine to prompt a Wireless Mouse whenever a Webcam is added to the cart, or launch a bundled discount campaign for both items to drive targeted cross-sell revenue.
