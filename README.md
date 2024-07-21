# CPE161
วิชาภาษา C

#include <stdio.h>

int main() {
    int c, s, u, v, t, a;  // ประกาศตัวแปรที่จำเป็น

    printf("Please select choice\n");
    printf("**********\n");
    printf("1. Find s #\n");
    printf("2. Find u #\n");
    printf("3. Find v #\n");
    printf("4. Find t #\n");
    printf("5. Find a #\n");
    printf("Select : ");
    scanf("%d", &c);

    switch (c) {
    case 1:
        printf("Please enter u : ");
        scanf("%d", &u);
        printf("Please enter t : ");
        scanf("%d", &t);
        printf("Please enter a : ");
        scanf("%d", &a);
        s = u * t + (a * t * t) / 2;
        printf("%d * %d + 1/2 * %d * %d * %d = %d\n", u, t, a, t, t, s);
        break;
    case 2:
        printf("Please enter v : ");
        scanf("%d", &v);
        printf("Please enter t : ");
        scanf("%d", &t);
        printf("Please enter a : ");
        scanf("%d", &a);
        u = v - a * t;
        printf("%d - %d * %d = %d\n", v, a, t, u);
        break;
    case 3:
        printf("Please enter u : ");
        scanf("%d", &u);
        printf("Please enter t : ");
        scanf("%d", &t);
        printf("Please enter a : ");
        scanf("%d", &a);
        v = u + a * t;
        printf("%d + %d * %d = %d\n", u, a, t, v);
        break;
    case 4:
        printf("Please enter v : ");
        scanf("%d", &v);
        printf("Please enter u : ");
        scanf("%d", &u);
        printf("Please enter t : ");
        scanf("%d", &t);
        s = 2 * s / (v + u);
        printf("2 * %d / (%d + %d) = %d\n", s, v, u, s);
        break;
    case 5:
        printf("Please enter v : ");
        scanf("%d", &v);
        printf("Please enter u : ");
        scanf("%d", &u);
        printf("Please enter t : ");
        scanf("%d", &t);
        a = (v - u) * t;
        printf("(%d - %d) * %d = %d\n", v, u, t, a);
        break;
    default:
        printf("Please select 1-5 only\n");
        break;
    }

    return 0;
}
