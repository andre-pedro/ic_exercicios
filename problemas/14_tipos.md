# Tipos compostos

## Enumerações

1 - Qual a saída do seguinte programa. Explica o teu raciocínio.

```c
#include <stdio.h>
enum dia {DOM = 1, SEG, TER, QUA, QUI, SEX, SAB};

int main()
{
    enum dia d = SEX;
    printf("Valor da variavel 'd': %d\n", d);
    return 0;
}
```

> [Soluções](../solucoes/14_tipos/01.md)

2 - Qual a saída do seguinte programa. Explica o teu raciocínio.

```c
#include <stdio.h>
enum situacao {ESTAVEL = 0, INSTAVEL, DESCONHECIDA};
enum situacao sitAtual = 2;

enum situacao obter_situacao() {
    return sitAtual;
}

void definir_situacao(enum situacao sit) {
    sitAtual = sit;
}

int main() {
   (obter_situacao() == ESTAVEL) ? printf("OK!\n") : printf("PROBLEMAS?!\n");
   definir_situacao(ESTAVEL);
   printf("Situacao: %d\n", obter_situacao());
   return 0;
}
```

> [Soluções](../solucoes/14_tipos/02.md)

## Estruturas

Em breve

## Definição de tipos

Em breve
