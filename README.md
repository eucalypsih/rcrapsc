# rcrapsc
[unsigned integer type with width of exactly 8, 16, 32 and 64 bits respectively (provided only if the implementation directly supports the type)](https://en.cppreference.com/w/c/types/integer)
```c
#include <stdio.h>
#include <stdint.h>

typedef struct students {
         uint8_t stuid;
} stu;

int main() {
        stu temp;
        temp.stuid = 1;
        printf("Temp: %hhu\n", sizeof(temp.stuid));
        return 0;
}
```

```c
#include <stdio.h>
#include <string.h

struct myStructures {
        int myNum;
        char myLetter;
        char myString[5];
};

int main(){
        struct myStructures s1;
        s1.myNum = 1;
        s1.myLetter = 'A';
        strcpy(s1.myString, "Some Text");
        printf("%d %c %s, s1.myNum, s1.myLetter, s1.myString);
        return 0;
}

```


