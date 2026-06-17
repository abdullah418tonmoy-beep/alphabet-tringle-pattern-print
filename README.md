#include <stdio.h>

int main()
{
    int n, i, j;

    scanf("%d", &n);

    for(i = 1; i <= n; i++)   // Row loop
    {
        int a = 1;            // প্রতিটি নতুন লাইনে A থেকে শুরু হবে

        for(j = 1; j <= i; j++)   // CHANGE: j<=n এর জায়গায় j<=i
        {
            int d = a + 64;       // 65 = A
            char ch = (char)d;

            printf(" %c ", ch);

            a++;
        }

        printf("\n");
    }

    return 0;
}
