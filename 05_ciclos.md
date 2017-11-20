# Ciclos

Soluções disponíveis [aqui](05_ciclos_sol.md).

**1 - Indique a saída produzida pelo seguinte programa em C:**

```c
#include <stdio.h>
int main() {
    unsigned int i;
    for (i = 8; i < 16; ++i) {
        printf("%x\n", i);
    }
    return 0;
}
```

**2 - Indique a saída produzida pelo seguinte programa em C:**

```c
#include <stdio.h>
int main() {
    unsigned int i;
    for (i = 5; i < 10; ++i) {
        printf("%o\n", i);
    }
    return 0;
}
```

**3 - Indique a saída produzida pelo seguinte programa em C:**

```c
#include <stdio.h>
int main() {
    unsigned int i;
    for (i = 0x0A; i < 0x12; ++i) {
        printf("%u\n", i);
    }
    return 0;
}
```

**4 - Indique a saída produzida pelo seguinte programa em C:**

```c
#include <stdio.h>
int main() {
    int i;
    for (i = 0; i <= 10; i += 2) {
        printf("%d\n", i);
    }
    return 0;
}
```
