python
import pandas as pd
from datetime import datetime, timedelta
#set random seed for reproducibility random. seed (42)
def generate_product_data (num_records=10)
Generate random product dataset with numerical data
Args: num_records(int): Number of product records to generate
Returns: pd. DataFrame: DataFrame containing product data
products = []
Categories = ['Electronics', 'Clothing', 'Home and Garden', 'Sports', 'Books']
for i in range (num-records) :
product = {
'product_id': 1000+i,
'category': random.choice(categories)
'price': round(random.uniform(10, 500),2),
'quantity_in_stock': random.randint(0, 500),
'units_sold':random.randint (0,1000),2),
'customer_rating':round(random.uniform(1.0, 5.0), 2)
'revenue' round (random.uniform(100,50000), 2)
'discount_percent':round(random.uniform(0,50),2),
'supplier_cost': round(random.uniform(5,250), 2),
'days_in_stock' random.randint(1,365)
}
products.append(product)
return pd DataFrame(products)
def save_to_csv(df, filename= 'product_data.csv):
"""Save dataset to CSV file."""
df.to_csv(filename, index=False)
print(f" Dataset saved to {filename} ")
def save_to_json(df, filename= 'product_data.json'):
"""Save dataset to JSON file."""
df.to_json(filename, orient='records', indent=2)
print(f Dataset saved to {filename}")
if __name__=="main":
#Generate dataset
print (Generating random product dataset...")
df= generate_product_data(num_records=10)
#Display the dataset"
print("\nDataset Preview:")
print (df)
print (f"\in Dataset shape:{df.shape}")
print (f"\ in Dataset info:")
print (df.info:())
print (f"\nDataset statistics:")
print (df.describe())
#Save to files
print("\nSaving dataset...")
save_to_csv(df)
save_to_json(df)
print("\n)
