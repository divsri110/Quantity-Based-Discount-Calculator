# Quantity-Based-Discount-Calculator
This program calculates the total expense for a purchase, applying a 10% discount if the quantity exceeds 1000 units. It takes quantity and rate as input, uses an if-else to determine the discount, then computes the final total after subtracting the discount amount.
#include <stdio.h>

int main (){

    int qty, dis;
    float rate, tot;

    printf("Enter the quantity and rate of item");
    scanf("%d%f", &qty, &rate);

    if (qty>1000)
           dis=10;

    else
           dis=0;

    tot=(qty*rate)-(qty*rate*dis/100);

    printf("Total Expense=%f", tot);

    return 0;

}
