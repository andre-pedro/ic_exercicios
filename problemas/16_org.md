# Organização de programas

1 - Cria um ficheiro `.c` que implemente as funções do seguinte ficheiro `.h`
(interface).

```c
enum tecla {
    TECLA_W     (1 << 0),
    TECLA_S     (1 << 1),
    TECLA_A     (1 << 2),
    TECLA_D     (1 << 3),
    TECLA_SPACE (1 << 4),
    TECLA_CTRL  (1 << 5),
    TECLA_SHIFT (1 << 6),
    TECLA_ALT   (1 << 7)
};

/* Atualiza estado com indicacao de que a tecla t esta' a ser pressionada. */
void tecla_pressionar(int *estado, enum tecla t);

/* Atualiza estado com indicacao de que a tecla t foi libertada. */
void tecla_libertar(int *estado, enum tecla t);

/* Testa se a tecla t esta' a ser pressionada ou nao. Devolve 1 caso a tecla
   esteja a ser pressionada ou 0 em caso contrario. */
int tecla_esta_pressionada(int estado, enum tecla t);
```

> [Soluções](../solucoes/16_org/01.md)

<a name="p2" />

2 - Considera a seguinte interface disponibilizada no ficheiro "rectangulo.h":

```c
/** Estrutura rectangulo. */
typedef struct {
    double x1; /**< Coordenada x do canto superior esquerdo. */
    double y1; /**< Coordenada y do canto superior esquerdo. */
    double x2; /**< Coordenada x do canto inferior direito.  */
    double y2; /**< Coordenada y do canto inferior direito.  */
} RECTANGULO;

/**
 * @brief Criar novo rectangulo.
 *
 * @param x1 Coordenada x do canto superior esquerdo.
 * @param y1 Coordenada y do canto superior esquerdo.
 * @param x2 Coordenada x do canto inferior direito.
 * @param y2 Coordenada y do canto inferior direito.
 * @return Um novo rectangulo.
 * */
RECTANGULO *rectangulo_new(double x1, double y1, double x2, double y2);

/**
 * @brief Destruir rectangulo.
 *
 * @param r Rectangulo a destruir.
 * */
void rectangulo_destroy(RECTANGULO *r);

/**
 * @brief Obtem a area de um rectangulo.
 *
 * @param r Rectangulo do qual obter a area.
 * */
double rectangulo_area(RECTANGULO *r);
```

Usando estas funcionalidades, escreve um programa, "testar_rectangulo.c", que
peça ao utilizador as coordenadas de um rectângulo e depois apresente no ecrã a
sua área.

> [Soluções](../solucoes/16_org/02.md)

<a name="p3" />

3 - Escreve um programa em C  (ficheiro "rectangulo.c") com uma possível
implementação da interface apresentada na pergunta anterior. A área de um
rectângulo é dada por `|x2 - x1| * |y2 - y1|` (onde se assume que `|x|` é o
módulo de `x`). A função `fabs()` (da biblioteca `math.h`), realiza a operação
módulo em _doubles_.

```c
#include "rectangulo.h"
#include <math.h>
#include <stdlib.h>
RECTANGULO *rectangulo_new(double x1, double y1, double x2, double y2) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
void rectangulo_destroy(RECTANGULO *r) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
double rectangulo_area(RECTANGULO *r) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```

> [Soluções](../solucoes/16_org/03.md)

<a name="p4" />

4 - A partir do código desenvolvido nos dois problemas anteriores, escreve uma
`Makefile` para criar uma _build_ do programa "testar_rectangulo.c".

> [Soluções](../solucoes/16_org/04.md)

<a name="p5" />

5 - Considera o problema [4](15_mem.md#p4) da secção
[Gestão dinâmica da memória](15_mem.md). Organiza o código de modo a que tenhas
um módulo composto por um ficheiro `.c` e por um ficheiro `.h` para gestão de
objetos do tipo `PLAYER`. Depois escreve uma `Makefile` para criar uma _build_
do programa para testar a funcionalidade do módulo (problema [5](15_mem.md#p5)
da mesma secção).

> [Soluções](../solucoes/16_org/05.md)
