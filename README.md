## Given the data, using **_owners_ and _vehicles_ tables**, complete the following exercises and put your submissions in the **queries.sql** document. 

### The queries
1. Join the two tables so that every column and record appears, regardless of if there is not an owner_id.

2. Count the number of cars for each owner. Display the owners first_name, last_name and count of vehicles. The first_name should be ordered in ascending order.

3. Count the number of cars for each owner and display the average price for each of the cars as integers. Display the owners first_name, last_name, average price and count of vehicles. The first_name should be ordered in descending order. Only display results with more than one vehicle and an average price greater than 10000.

### The data

#### Owners

owners (id SERIAL PRIMARY KEY, first_name TEXT, last_name TEXT)

#### Vehicles

vehicles (id SERIAL PRIMARY KEY, make TEXT, model TEXT, year INTEGER, price REAL, owner_id INTEGER REFERENCES owners (id));