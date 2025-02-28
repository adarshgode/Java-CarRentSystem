The Car Rental System is a console-based application developed in Java, designed to facilitate the process of renting cars. This application allows customers to rent available cars, calculate rental costs based on the rental period, and return cars after use. It includes functionalities for managing car availability, tracking rentals, and maintaining customer information.

Features
Car Management: Add new cars with unique IDs, brand names, models, and base rental prices per day.
Customer Management: Register new customers and store their information.
Rental Process: Rent available cars to customers and calculate the total rental price based on the number of rental days.
Return Process: Return rented cars and update their availability status.
User-Friendly Menu: Simple and intuitive console-based menu for interacting with the system.
Classes and Their Responsibilities

Car:
Attributes: carId, brand, model, basePricePerDay, isAvailable
Methods: Constructor, getters, calculatePrice(), isAvailable(), rent(), returnCar()

Customer:
Attributes: customerId, name
Methods: Constructor, getters

Rental:
Attributes: car, customer, days
Methods: Constructor, getters

CarRentalSystem:
Attributes: cars, customers, rentals
Methods: addCar(), addCustomer(), rentCar(), returnCar(), menu()

Main:
Initializes the CarRentalSystem and adds sample cars.
Starts the menu-driven interaction with the user.
How to Use
Run the Program: Execute the Main class to start the application.
Menu Options:
Rent a Car: Enter customer name, select a car from the list of available cars, and specify the rental duration to calculate the total price. Confirm the rental to finalize the transaction.
Return a Car: Enter the car ID to return the rented car and update its availability status.
Exit: Terminate the application.
Sample Execution
The user is presented with a menu to rent a car, return a car, or exit.
On selecting "Rent a Car", the user is prompted to enter their name, choose a car from the available list, and provide the number of rental days. The system calculates and displays the total rental price, and the user can confirm the rental.
On selecting "Return a Car", the user is prompted to enter the car ID of the rented car to complete the return process.
Project Structure
lua
Copy code
CarRentalSystem/
|-- src/
|   |-- Car.java
|   |-- Customer.java
|   |-- Rental.java
|   |-- CarRentalSystem.java
|   |-- Main.java
|-- README.md
Getting Started
Clone the Repository:
bash
Copy code
git clone https://github.com/yourusername/CarRentalSystem.git
Navigate to the Project Directory:
bash
Copy code
cd CarRentalSystem
Compile the Source Files:
css
Copy code
javac src/*.java
Run the Application:
css
Copy code
java src.Main
Future Enhancements
Implement a graphical user interface (GUI) for a better user experience.
Add database integration to persist data across sessions.
Include more detailed rental records and history tracking.
Introduce user authentication and authorization.


Conclusion
The Car Rental System is a foundational project that showcases object-oriented programming principles and basic file handling in Java. It provides a practical solution for managing car rentals and can be extended with additional features and functionalities for more complex scenarios.
