# System-to-find-length-of-string-ang-copying-1-string-into-another-without-built-in
Basic c-program to find length of string ang copying 1 string into another without built in
#include <stdio.h>

int main() {
    char str1[100], str2[100];
    int i, len = 0;

    printf("Enter a string: ");
    fgets(str1, sizeof(str1), stdin);   

   
    for(i = 0; str1[i] != '\0' && str1[i] != '\n'; i++) {
        len++;
    }
    printf("Length = %d\n", len);

   
    for(i = 0; str1[i] != '\0' && str1[i] != '\n'; i++) {
        str2[i] = str1[i];
    }
    str2[i] = '\0';

    printf("Copied string = %s\n", str2);

    return 0;
}

