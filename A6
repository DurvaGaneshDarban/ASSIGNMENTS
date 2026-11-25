#include <stdio.h>

unsigned long long factorial_iterative(int n) {
    unsigned long long result = 1;
    for (int i = 2; i <= n; i++) {
        result *= (unsigned long long)i;
    }
    return result;
}

unsigned long long factorial_recursive(int n) {
    if (n <= 1) {
        return 1ULL;
    }
    return (unsigned long long)n * factorial_recursive(n - 1);
}

int main(void) {
    int n;
    printf("Enter a non-negative integer: ");
    if (scanf("%d", &n) != 1 || n < 0) {
        printf("Invalid input. Please enter a non-negative integer.\n");
        return 1;
    }

    unsigned long long iter_fact = factorial_iterative(n);
    unsigned long long rec_fact = factorial_recursive(n);

    printf("Factorial of number (without recursion) = %llu\n", iter_fact);
    printf("Factorial of number (with recursion) = %llu\n", rec_fact);

    return 0;
}
