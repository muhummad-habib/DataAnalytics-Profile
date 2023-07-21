# E-Commerce DataBase Exploration with MySQL & Python

This project explores an E-Commerce database using MySQL and Python for data analysis and visualization. The database contains tables for orders, order details, users, and categories. The project uses the 'mysql-connector-python' package to connect to the MySQL database and the 'pandas', 'numpy', 'matplotlib', and 'seaborn' packages for data analysis and visualization.

## MySQL Setup

1. Install the required packages:
```bash
!pip install mysql-connector-python
!pip install ipython-sql
```

3. Load the 'ipython-sql' extension in your Jupyter Notebook:
```bash
%load_ext sql
```

4. Establish a connection to the MySQL database:
```bash
import mysql.connector
from mysql.connector import Error
```
```bash
user_name = os.environ.get('DB_USER')
password = os.environ.get('DB_PASS')
```

#### Create a connection to the database
```bash
conn = mysql.connector.connect(
    host='127.0.0.1',
    user=user_name,
    passwd=password,
    db='e_commerce_db'
)
```
#### Check if the connection was successful
```bash
if conn.is_connected():
    print("Connected to the MySQL database.")
```
#### Register the connection with ipython-sql:
```bash
%sql mysql+mysqlconnector://{user_name}:{password}@localhost/e_commerce_db
```
## Business Questions
The project answers the following business questions using SQL queries and Python visualizations:

- Find all profitable orders.
- Find the customer who has placed the maximum number of orders.
- Identify the most profitable category.
- Identify the most profitable state.
- Find all categories with profit higher than 5000.
- Rank customers based on their total order amounts.
- Rank categories based on their total profits.
- Find the top 5 customers with the highest average order amounts.
- Find the top 5 categories with the highest average profits.
- Calculate the cumulative sum of profits for each category over time.
  
## Project Structure
The project consists of the following files:

- MySQL and Python -- E_Commerce_DB_Exploration.ipynb: 
Jupyter Notebook containing the SQL queries, Python code, and visualizations.
- data/: Folder containing the E-Commerce database dump file.
- README.md: Project documentation.
## Getting Started
- Clone the repository to your local machine.
- Restore the E-Commerce database using the dump file in the data/ folder.
- Set up your MySQL credentials in the Jupyter Notebook to establish a connection to the database.
- Run the Jupyter Notebook to explore and analyze the E-Commerce database.
### Dependencies
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- mysql-connector-python

## Contact Information

For any questions or inquiries, please contact:

##### Muhammad Habib

[muhummad.habib7@gmail.com](muhummad.habib7@gmail.com)

LinkedIn: [linkedin.com/in/muhammad-habib](https://www.linkedin.com/in/muhammad-habib)
