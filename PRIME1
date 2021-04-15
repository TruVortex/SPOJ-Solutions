// brute force prime check > sieve i guess
#include <stdio.h>
#include <math.h>
#define scan(x) do{while((x=getchar())<'0'); for(x-='0'; '0'<=(_=getchar()); x=(x<<3)+(x<<1)+_-'0');}while(0)
char _;

using namespace std;

bool prime(int n) {
    if (n == 1) {
        return false;
    }
    if (n % 2 == 0) {
        return false;
    }
    for (int i = 3; i <= sqrt(n); i += 2) {
        if (n % i == 0) {
            return false;
        }
    }
    return true;
}

int main() {
    int t;
    scan(t);
    for (int i = 0; i < t; i++) {
        int m, n;
        scan(m);
        scan(n);
        if (m <= 2) {
            printf("2\n");
        }
        if (m % 2 == 0) {
            m++;
        }
        for (int i = m; i <= n; i += 2) {
            if (prime(i)) {
                printf("%d\n", i);
            }
        }
        printf("\n");
    }
    return 0;
}
