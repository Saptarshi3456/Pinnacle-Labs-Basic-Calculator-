# Pinnacle-Labs-Basic-Calculator-
It is a basic calculator which do basic algorithms like addition , subtraction, multiplication and division.

#include <stdio.h>
#include <math.h>

int main() {
    int choice, num1, num2;
    float result;

    printf("Simple Calculator\n");
    printf("---------------\n");

    printf("Menu\n");
    printf("----\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("5. Exit\n");
    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch (choice) {
        case 1:
            printf("Enter two numbers: ");
            scanf("%d %d", &num1, &num2);
            result = num1 + num2;
            printf("Result: %.2f\n", result);
            break;
        case 2:
            printf("Enter two numbers: ");
            scanf("%d %d", &num1, &num2);
            result = num1 - num2;
            printf("Result: %.2f\n", result);
            break;
        case 3:
            printf("Enter two numbers: ");
            scanf("%d %d", &num1, &num2);
            result = num1 * num2;
            printf("Result: %.2f\n", result);
            break;
        case 4:
            printf("Enter two numbers: ");
            scanf("%d %d", &num1, &num2);
            if (num2 != 0) {
                result = (float)num1 / num2;
                printf("Result: %.2f\n", result);
            } else {
                printf("Error: Division by zero\n");
            }
            break;
        case 5:
            printf("Exiting...\n");
            return 0;
        default:
            printf("Invalid choice\n");
    }

    return 0;
}
