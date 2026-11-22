# Car Rental Management System


## Project Overview

The system models a small car rental service. It keeps track of cars, customers, rental availability, cars rented by each customer, and rental fee records.

### Features

- Store car details such as car ID, make, model, and manufacturing year.
- Store customer details and the cars rented by each customer.
- Rent a car only when it is available.
- Prevent a car from being rented again while it is marked unavailable.
- Return a car and update its availability.
- Display each customer's rented cars.
- Maintain rental records with rental IDs and rental fees.

## Technologies Used

- **Language:** Python 3
- **Environment:** Jupyter Notebook (for `My_Project.ipynb`) or a Python terminal (for `main.py`)
- **Libraries:** Python standard library only

## Repository Structure

```text
Car_Rental_Management_System/
│
├── main.py              # OOP implementation
├── My_Project.ipynb     # Dictionary-and-function implementation
├── requirements.txt     # Project dependencies
├── .gitignore           # Files excluded from Git
└── README.md            # Project documentation
```

**Main workflow:**

1. Create a list of cars.
2. Create a list of customers.
3. Customers rent available cars.
4. Display the cars rented by each customer.
5. Selected customers return their cars.
6. Display the updated rented-car lists.
7. Create and display rental fee records.

### Notebook implementation (`My_Project.ipynb`)

The notebook uses dictionaries to represent cars and customers. Functions handle renting and returning cars, and a list stores rental records.

| Function | Purpose |
|---|---|
| `rent_car(customer, car)` | Checks availability, marks the car unavailable, and adds it to the customer's rented cars. |
| `return_car(customer, car)` | Returns a car if it belongs to that customer's rented-car list, then marks it available. |

## Concepts Demonstrated

- Variables and data types
- Lists and dictionaries
- Conditional statements
- Loops
- Functions
- Classes and objects
- Constructors (`__init__`)
- Object attributes and methods
- Basic object relationships
- State and availability management
- Formatted output using f-strings

## Sample Output

The exact output depends on which implementation you run. The OOP script displays rented-car lists, updated lists after returns, and rental information. Example format:

```text
Adarsh Wahewal's Rented Cars: ['Toyota']
Rental ID:R001,Customer:Adarsh Wahewal,Car:Toyota, Rental Fee:INR 5000.0
```

## Current Scope and Limitations

This is a basic, in-memory learning project:
- Data is stored in Python lists and objects/dictionaries; it is not saved to a database or file.
- The project does not provide a graphical user interface or web interface.
- Rental dates, return dates, late fees, and payment processing are not implemented.
- The `Rental` records are created separately from the rent/return operations in the OOP script. They are demonstration records, not a persistent transaction history.
- The two implementations use different sample data and rental fees.

## Future Improvements

- Add a menu-driven interface.
- Add search, add, and remove operations for cars and customers.
- Validate unique car, customer, and rental IDs.
- Connect rental records directly to successful rent and return operations.
- Add rental start dates, due dates, and late-fee calculations.
- Store data using SQLite or MySQL.
- Add unit tests and input validation.
- Build a web interface using Flask or Django.

## Learning Objective

The objective of this project is to understand how a simple real-world car rental workflow can be implemented in Python, first with dictionaries and functions and then with classes and objects.
