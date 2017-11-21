# Controlo de fluxo

1 - Indique a saída produzida pelo seguinte programa em C:

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

> [Soluções](../solucoes/06_controlofluxo/01.md)

2 - Indique a saída produzida pelo seguinte programa em C:

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

> [Soluções](../solucoes/06_controlofluxo/02.md)

3 - Indique a saída produzida pelo seguinte programa em C:

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

> [Soluções](../solucoes/06_controlofluxo/03.md)

4 - Indique a saída produzida pelo seguinte programa em C:

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

> [Soluções](../solucoes/06_controlofluxo/04.md)


5 - Indique a saída produzida pelo seguinte programa em C:

```c
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d", &a);
    scanf("%d", &b);
    if (a > b) {
        printf("Valor 'a' maior que 'b'\n");
    } else if (a < b) {
        printf("Valor 'a' menor que 'b'\n");
    } else {
        printf("So podem ser iguais\n");
    }
    return 0;
}
```

> [Soluções](../solucoes/06_controlofluxo/05.md)
