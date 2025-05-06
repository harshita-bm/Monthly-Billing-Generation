📊 Monthly Billing Generation
This project automates the process of generating monthly billing summaries based on a list of furniture and facility usage items. It calculates the billable amount for each item based on its active days in a given month, quantity, and rate. The solution groups similar items together and provides a clean output with the total revenue for that month.

🔧 What It Does
Accepts an input list of items, each with:

item_code: Name of the item (e.g., Executive Desk, Parking).

qty: Quantity being billed.

rate: Rate per item.

start_date and stop_date: Time period during which the item was used.

Filters items that are active during the target month.

Calculates prorated amounts if items were not active for the full month.

Groups items by item code and rate.

Outputs a list of grouped billing entries along with total revenue.

📥 Input
You provide a list of dictionaries in Python where each dictionary represents an item usage entry. This input can be easily copied into a Jupyter notebook cell.

📤 Output
The code returns a dictionary with:

line_items: Grouped and summarized entries per item.

total_revenue: The sum of all billable amounts.

The result is also printed in a pretty JSON format for easy reading.

📘 How to Run
Open the .ipynb notebook in Jupyter.

Ensure your item list and target month (e.g., "2024-11") are passed to the function.

Run all cells to see the formatted output.

🛠️ Tools Used
Python Standard Libraries: datetime, collections, calendar, json

Jupyter Notebook: For interactive development and testing

💡 Use Cases
Monthly office space rental billing

Prorated invoicing for shared resources

Dynamic billing reports based on time usage
