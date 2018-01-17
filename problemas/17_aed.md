1 - Completa a seguinte função cujo objetivo é embaralhar (_shuffle_) os
conteúdos do array de apontadores genéricos passado como primeiro argumento.
Existem várias formas de embaralhar um array, sendo o algoritmo de [Fisher–Yates](https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle) um
dos mais utilizados.


```c
void shuffle(void *array[], int tamanho) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```

> [Soluções](../solucoes/17_aed/01.md)

2 - Considera os problemas [2](16_org.md#p2), [3](16_org.md#p3) e
[4](16_org.md#p4) da secção [Organização de programas](16_org.md). Adiciona uma
função nova ao módulo "rectangulo" que retorne 1 caso o primeiro rectângulo
esteja completamente contido dentro do segundo rectângulo, e 0 em caso
contrário. Adiciona forma de testar esta função ao programa
"testar_rectangulo.c". O protótipo da nova função pode ser o seguinte:

```c
/**
 * @brief Indica se o primeiro rectangulo esta' contido dentro do segundo
 * rectangulo.
 *
 * @param r1 Rectangulo a verificar se esta contido dentro de `r2`.
 * @param r2 Rectangulo que possivelmente contem `r1`.
 * @return Um caso `r1` esteja totalmente contido dentro de `r2`, ou zero caso
 * contrario.
 * */
int rectangulo_esta_contido(RECTANGULO *r1, RECTANGULO *r2);
```

> [Soluções](../solucoes/17_aed/02.md)


3 - Completa a seguinte função, que recebe um array de inteiros e ordena-o de
forma ascendente usando
[Bubble sort](https://en.wikipedia.org/wiki/Bubble_sort).

```c
void sort_ints(int *array, int tamanho) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```
> [Soluções](../solucoes/17_aed/03.md)


4 - Completa a seguinte função, que recebe um array de _doubles_ e devolve um
novo array de _doubles_ ordenado de forma ascendente. Usa o
[Selection sort](https://en.wikipedia.org/wiki/Selection_sort) e explica porque
neste caso é necessário criar um novo array.

```c
double *sort_doubles(double *array_in, int tamanho) {

    double *array_out;

    /* ************ */
    /* Codigo aqui! */
    /* ************ */

    return array_out;
}
```

> [Soluções](../solucoes/17_aed/04.md)

5 - O ficheiro "fila.h" mostrado em baixo constitui uma interface para uma
estrutura de dados para tipos genéricos chamada
[Fila](https://en.wikipedia.org/wiki/Queue_(abstract_data_type)), na qual o
primeiro objeto a entrar é o primeiro a sair. Escreve o código do ficheiro
"fila.c" que implementa esta interface.

```c
#ifndef FILA_H
#define FILA_H

typedef struct fila FILA;

struct fila {
    void *item;
    FILA *next;
};

void fila_insere(FILA **aaf, void *item);

void *fila_retira(FILA **aaf);

unsigned int fila_tamanho(FILA *af);

#endif
```

> [Soluções](../solucoes/17_aed/05.md)
