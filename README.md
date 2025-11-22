FUEL TANK MANAGEMENT SYSTEM
C Programming Console Application
ABSTRACT

The Fuel Tank Management System is a console-based application developed using the C programming language. Its primary purpose is to simulate the management of a vehicle’s fuel tank by allowing the user to check fuel status, add fuel, and consume fuel through a menu-driven interface.

The system uses a structure (struct) to store tank attributes such as capacity and current fuel level. It demonstrates essential programming concepts including structures, functions, pointers, decision-making, and loops, making it an ideal beginner-level project.

The program ensures safe and realistic tank operations by validating fuel input and preventing overfilling or overconsumption.

FUNCTIONAL REQUIREMENTS
1. Show Fuel Status

Displays the current state of the fuel tank.

Shows:

Tank Capacity

Current Fuel Level

2. Add Fuel

Allows the user to add fuel to the tank.

Input:

Amount of fuel to add (liters)

Validation:

Amount must be greater than 0

Added fuel cannot exceed tank capacity

Displays updated fuel level on success

3. Use Fuel (Consume Fuel)

Allows fuel consumption from the tank.

Input:

Amount of fuel to use (liters)

Validation:

Amount must be greater than 0

Cannot use more fuel than available

Displays updated fuel level on success

4. Exit Program

Closes the application safely.

PROJECT FEATURES
✔ Structure-Based Data Storage

A FuelTank structure stores:

capacity      // maximum fuel capacity
currentFuel   // current fuel level

✔ Menu-Driven Interface

Simple and easy-to-use options:

1. Show Fuel Status
2. Add Fuel
3. Use Fuel
4. Exit

✔ Input Validation

Handles incorrect or dangerous operations:

Negative or zero fuel amounts

Overflow beyond tank capacity

Using more fuel than available

✔ Modular Programming

Uses separate functions for:

showStatus()

addFuel()

useFuel()

✔ Pointer Usage

Fuel modification uses pointer-based function calls for direct structure updating.

SCREENSHOTS OF OUTPUT (TEXT SIMULATION)

(Console-style sample outputs)

Screenshot 1: Setting Tank Capacity
Enter tank capacity (liters): 50

Screenshot 2: Main Menu
==== Fuel Management Menu ====
1. Show Fuel Status
2. Add Fuel
3. Use Fuel
4. Exit
Choose an option: _

Screenshot 3: Adding Fuel
Enter amount to add: 20
Successfully added 20.00 liters. Current fuel: 20.00 liters

Screenshot 4: Overfilling Attempt
Enter amount to add: 40
Cannot add 40.00 liters. It exceeds tank capacity!

Screenshot 5: Showing Fuel Status
--- Fuel Status ---
Tank Capacity : 50.00 liters
Current Fuel  : 20.00 liters
-------------------

Screenshot 6: Using Fuel
Enter amount to use: 10
Used 10.00 liters. Remaining fuel: 10.00 liters

Screenshot 7: Not Enough Fuel
Enter amount to use: 30
Not enough fuel! Available: 10.00 liters

Screenshot 8: Exit Program
Exiting program...
