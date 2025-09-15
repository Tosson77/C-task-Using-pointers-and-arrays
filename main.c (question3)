
#include <stdio.h>

char* my_strstr(const char* str, const char* sub) {
    while (*str) {
        const char* s1 = str;
        const char* s2 = sub;
        while (*s1 && *s2 && *s1 == *s2) {
            s1++;
            s2++;
        }
        if (!*s2)
            return (char*)str;
        str++;
    }
    return NULL;
}

int main() {
    const char* text = "Formula Student Egypt";
    const char* word = "Student";

    char* result = my_strstr(text, word);
    if (result)
        printf("Found: %s\n", result);
    else
        printf("Not found\n");

    return 0;
}
