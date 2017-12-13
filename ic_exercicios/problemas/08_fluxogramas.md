# Fluxogramas

1 - Desenha o fluxograma do seguinte programa:

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

> [Soluções](../solucoes/08_fluxogramas/01.md)

2 - Desenha o fluxograma do seguinte programa:

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

> [Soluções](../solucoes/08_fluxogramas/02.md)

3 - Desenha o fluxograma do seguinte programa:

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

> [Soluções](../solucoes/08_fluxogramas/03.md)

4 - Desenha o fluxograma do seguinte programa:

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

> [Soluções](../solucoes/08_fluxogramas/04.md)

5 - Desenha o fluxograma do seguinte programa:

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

> [Soluções](../solucoes/08_fluxogramas/05.md)

6 - Desenha o fluxograma do seguinte programa:

```c
#include <stdio.h>

/* Protótipos das funções. */
int funcao2(int i, int j);
void funcao1(int a, int b);

/* Função principal. */
int main() {
    int x = 1, y = 2, z = 3;
    funcao1(x, y);    
    printf("%d\t%d\t%d\n", x, y, z);
}

/* Corpos das funções. */
int funcao2(int i, int j) {
    int y = i + 1;
    int z = j + 1;
    printf("%d\t%d\n", y, z);
    return y + z;
}

void funcao1(int a, int b) {
    int x = -1, y = -2, z = -3;
    x += funcao2(a, b);
    printf("%d\t%d\t%d\n", x, y, z);
}
```

> [Soluções](../solucoes/08_fluxogramas/06.md)
