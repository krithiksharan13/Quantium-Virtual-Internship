# Forage Quantium Data Analytics Virtual Experience Program
Tasks Assigned: 
- Data preparation and customer analytics,
- Experimentation and uplift testing, and
- Analytics and commercial application.

## Dependencies
Language: Python 3.8 \
Packages: pandas, matplotlib, mlxtend, datetime, sklearn, scipy

## Project Overview and Task Insights 
This virtual experience program focuses on analyzing chip purchases at supermarkets. The project's goal was to assess customer purchasing behaviors and evaluate the performance of trial stores with a new layout. The findings provide insights into customer preferences and determine whether the trial was successful, along with a recommendation for the client.

### Task 1: Data Preparation and Customer Analytics
Files:
QVI_task1.ipynb: Reads QVI_purchase_behaviour.csv and QVI_transaction_data.xlsx
Data Cleaning:
- Converted date from integer format to datetime data type
- Removed salsas and outliers
- Analysis of Customer Purchase Behaviors:

Examined total sales, grouped by:
- LIFESTAGE: Categorizes customers based on family status and life stage
- MEMBER_TYPE: Segments shoppers based on product price points and purchasing preferences, identifying whether they prioritize quality/brand or opt for the cheapest options
- 
Deep Dive:
Focused on the Mainstream Young Singles/Couples segment to analyze their preferences in chip brand and packet size compared to other customer segments.

Insights:
- The three highest-contributing segments to total sales are:
  - 1.Budget Older Families
  - 2.Mainstream Young Singles/Couples
  - 3.Mainstream Retirees
- Older Families purchase the highest average number of chip packets per customer, while Mainstream Young Singles/Couples make up the largest customer population.
- Across most segments, Kettle Chips and 175g packets are the most frequently purchased.
- Mainstream Young Singles/Couples are 28% more likely to buy Tyrrells Chips than other segments and 32% more likely to purchase 270g chip packets, which are Twisties Chips.

### Task 2: Experimentation and Uplift Testing
Files: QVI_task2.ipynb, reads QVI_data.csv
- Three stores (77, 86, 88) undergo a new store layout with the trial period in Feb-Apr 2019
- Used the total sales and number of customers metric to generate a combined score to compare the trial and potential control stores with using Pearson correlations and magnitude distances
- Determined if difference in performance of those metrics of the control stores (stores with the highest score) compared to the trial store is significant using hypothesis testing 

Insights:
- Control and trial store pairs are:
  - 77 and 233
  - 86 and 155
  - 88 and 40
- For the total sales, store 77 saw a statistically significant increase (above the 95% control threshold) in Mar and Apr while store 86 saw an increase in Mar
- For the number of customers, both stores 77 and 86 saw significant increases in at least 2 months
- No significant change in performance due to the trial in store 88

### Task 3: Analytics and commercial application
- Prepared a report in Powerpoint highlighting key insights from Tasks 1 and 2 using the Pyramid Principle


