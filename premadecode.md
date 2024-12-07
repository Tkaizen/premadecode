
#include <stdio.h>

void check_logic(int a, int b) {
    printf("Checking logical operations for a = %d and b = %d\n", a, b);

    // AND operation (a && b)
    printf("a AND b: %d && %d = %d\n", a, b, a && b);

    // OR operation (a || b)
    printf("a OR b: %d || %d = %d\n", a, b, a || b);

    // NOT operation on a (!a)
    printf("NOT a: !%d = %d\n", a, !a);

    // NOT operation on b (!b)
    printf("NOT b: !%d = %d\n", b, !b);
}

int main() {
    int a, b;

    // Get user input for two Boolean values (either 0 or 1)
    printf("Enter two Boolean values (0 or 1) for a and b:\n");
    printf("Enter value for a: ");
    scanf("%d", &a);
    printf("Enter value for b: ");
    scanf("%d", &b);

    // Ensure the input is valid (either 0 or 1)
    if ((a != 0 && a != 1) || (b != 0 && b != 1)) {
        printf("Invalid input. Please enter values 0 or 1 for a and b.\n");
        return 1;
    }

    // Call the function to check logic
    check_logic(a, b);

    return 0;
}
