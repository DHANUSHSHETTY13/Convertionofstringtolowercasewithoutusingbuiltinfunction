# Convertionofstringtolowercasewithoutusingbuiltinfunction
#include <stdio.h>

void toLowerCase(char *str) {
    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] >= 'A' && str[i] <= 'Z') {
            str[i] = str[i] + 32;
        }
    }
}

int main() {
    char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    toLowerCase(str);

    printf("String in lowercase: %s\n", str);

    return 0;
}
