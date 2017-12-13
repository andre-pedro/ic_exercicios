# Funções

1 - O que é impresso no ecrã pelo seguinte programa em C?

```c
#include <stdio.h>

void func(unsigned char * y) {
    unsigned char x = ++(*y) - 6;
    printf("%u ", x);
}

int main() {
    unsigned char x = 4;
    func(&x);    
    printf("%u\n", x);
}
```

> [Soluções](../solucoes/07_funcoes/01.md)

2 - O que é impresso no ecrã pelo seguinte programa em C?

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

> [Soluções](../solucoes/07_funcoes/02.md)

3 - O que é impresso no ecrã pelo seguinte programa em C?

```c
#include <stdio.h>

void recursiva(int valor) {
    if (valor == 0) {
        printf("Fim!\n");
    } else {
    	printf("%d\n", valor);
        recursiva(valor - 1);
    }
}

int main() {
    int x = 5;
    recursiva(x);
}
```

> [Soluções](../solucoes/07_funcoes/03.md)
