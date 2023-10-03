#include <stdio.h>

int main() {
    int n = 6;  // 定义爱心的大小，可以根据需要调整

    // 打印爱心上半部分
    for (int i = n/2; i <= n; i += 2) {
        // 控制每行的空格数
        for (int j = 1; j < n-i; j += 2) {
            printf(" ");
        }

        // 控制每行的爱心符号数
        for (int j = 1; j <= i; j++) {
            printf("*");
        }

        // 控制每行的空格数
        for (int j = 1; j <= n-i; j++) {
            printf(" ");
        }

        // 控制每行的爱心符号数
        for (int j = 1; j <= i; j++) {
            printf("*");
        }

        printf("\n");
    }

    // 打印爱心下半部分
    for (int i = n; i >= 1; i--) {
        // 控制每行的空格数
        for (int j = i; j < n; j++) {
            printf(" ");
        }

        // 控制每行的爱心符号数
        for (int j = 1; j <= (i*2)-1; j++) {
            printf("*");
        }

        printf("\n");
    }

    return 0;
}
