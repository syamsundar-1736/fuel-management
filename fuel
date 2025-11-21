#include <stdio.h>

// Structure to represent a fuel tank
typedef struct {
    float capacity;      // Maximum tank capacity
    float currentFuel;   // Current fuel level
} FuelTank;

// Display fuel status
void showStatus(FuelTank tank) {
    printf("\n--- Fuel Status ---\n");
    printf("Tank Capacity : %.2f liters\n", tank.capacity);
    printf("Current Fuel  : %.2f liters\n", tank.currentFuel);
    printf("-------------------\n");
}

// Add fuel to the tank
void addFuel(FuelTank *tank, float amount) {
    if (amount <= 0) {
        printf("Invalid amount! Must be greater than 0.\n");
        return;
    }

    if (tank->currentFuel + amount > tank->capacity) {
        printf("Cannot add %.2f liters. It exceeds tank capacity!\n", amount);
    } else {
        tank->currentFuel += amount;
        printf("Successfully added %.2f liters. Current fuel: %.2f liters\n",
               amount, tank->currentFuel);
    }
}

// Use or consume fuel
void useFuel(FuelTank *tank, float amount) {
    if (amount <= 0) {
        printf("Invalid amount! Must be greater than 0.\n");
        return;
    }

    if (amount > tank->currentFuel) {
        printf("Not enough fuel! Available: %.2f liters\n",
               tank->currentFuel);
    } else {
        tank->currentFuel -= amount;
        printf("Used %.2f liters. Remaining fuel: %.2f liters\n",
               amount, tank->currentFuel);
    }
}

int main() {
    FuelTank tank;
    int choice;
    float amount;

    // Set tank capacity
    printf("Enter tank capacity (liters): ");
    scanf("%f", &tank.capacity);

    // Start with empty tank
    tank.currentFuel = 0;

    while (1) {
        printf("\n==== Fuel Management Menu ====\n");
        printf("1. Show Fuel Status\n");
        printf("2. Add Fuel\n");
        printf("3. Use Fuel\n");
        printf("4. Exit\n");
        printf("Choose an option: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                showStatus(tank);
                break;

            case 2:
                printf("Enter amount to add: ");
                scanf("%f", &amount);
                addFuel(&tank, amount);
                break;

            case 3:
                printf("Enter amount to use: ");
                scanf("%f", &amount);
                useFuel(&tank, amount);
                break;

            case 4:
                printf("Exiting program...\n");
                return 0;

            default:
                printf("Invalid choice! Please try again.\n");
        }
    }

    return 0;
}
