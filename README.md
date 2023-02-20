# c-program
#include <stdio.h>

int main() {
    int n, i, lowest;
    printf("Enter the number of integers: ");
    scanf("%d", &n);
    printf("Enter %d integers: ", n);
    scanf("%d", &lowest); //initialize lowest with the first integer
    for (i = 1; i < n; i++) {
        int num;
        scanf("%d", &num);
        if (num < lowest) {
            lowest = num; //update lowest if the current integer is smaller
        }
    }
    printf("Lowest is %d\n", lowest);
    return 0;
}
