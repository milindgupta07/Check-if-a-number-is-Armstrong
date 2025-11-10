# Check-if-a-number-is-Armstrong
Using C language program is made which gives the output to check if a number is armstrong or not
#include <stdio.h>
int main() {
    int num, temp, sum = 0;
    scanf("%d", &num);
    temp = num;
    while(temp > 0) {
        int d = temp % 10;
        sum += d * d * d;
        temp /= 10;
    }
    printf(sum == num ? "Armstrong" : "Not Armstrong");
    return 0;
}
