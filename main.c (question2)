#include <stdio.h>
#include <stdlib.h>

int main() {
    int n;
    printf("Enter size of matrix: ");
    fflush(stdout);
    scanf("%d", &n);

    int* A = (int*)malloc(n * n * sizeof(int));
    int* B = (int*)malloc(n * n * sizeof(int));
    int* C = (int*)malloc(n * n * sizeof(int));

    printf("Enter elements of A:\n");
    fflush(stdout);
    for (int i = 0; i < n*n; i++)
        scanf("%d", A + i);

    printf("Enter elements of B:\n");
    fflush(stdout);
    for (int i = 0; i < n*n; i++)
        scanf("%d", B + i);


    for (int i = 0; i < n*n; i++)
        *(C + i) = 0;


    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            for (int k = 0; k < n; k++) {
                *(C + i*n + j) += (*(A + i*n + k)) * (*(B + k*n + j));
            }
        }
    }

    printf("Result matrix:\n");
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++)
            printf("%d ", *(C + i*n + j));
        printf("\n");
    }

    free(A);
    free(B);
    free(C);
    return 0;
}

