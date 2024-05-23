// calculator
#include <stdio.h>
int main() {
    char choice;
    int x, y, z;

    printf("plz enter + to sum \n");
    printf("plz enter - to sub \n");
    printf("plz enter * to mult \n");
    printf("plz enter / to div \n");
    printf("plz enter 0 to exit \n");
    printf("----------------------- \n");
    printf("plz enter your choice \n");

    scanf(" %c", &choice);

    while (choice!= '0') {
        printf("plz enter 2 number to do that operation on it \n");
        scanf("%d %d", &x, &y);

        switch (choice) {
            case '+':
                z = x + y;
                printf("%d + %d = %d\n", x, y, z);
                break;
            case '-':
                z = x - y;
                printf("%d - %d = %d\n", x, y, z);
                break;
            case '*':
                z = x * y;
                printf("%d * %d = %d\n", x, y, z);
                break;
            case '/':
                if (y == 0) {
                    printf("Error: Division by zero\n");
                } else {
                    if (x/y==0)
                    printf("Error: Division by zero\n");
                    else{
                    z = x / y;
                    printf("%d / %d = %d\n", x, y, z);
                    }
                }
                break;
        }

        printf("plz enter your choice \n");
        scanf(" %c", &choice);
    }

    return 0;
}
