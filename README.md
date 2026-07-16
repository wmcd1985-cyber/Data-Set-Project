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
'price': round(random.uniform(10,500),2),
