# Linear-#include <stdio.h>
#define MAX 100

int queue[MAX], front = 0, rear = -1;

int main() {
    int n, val;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    for(int i = 0; i < n; i++) {
        printf("Enter value: ");
        scanf("%d", &val);
        queue[++rear] = val;
    }

    printf("Front element: %d", queue[front]);

    return 0;
}
