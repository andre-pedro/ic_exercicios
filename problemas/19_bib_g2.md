1 - Qual é a opção que é necessário passar ao compilador na fase de ligação
para construir programas que façam uso da biblioteca g2?

> [Soluções](../solucoes/19_bib_g2/01.md)

2 - Explica o que é desenhado pelo seguinte código C que faz uso da biblioteca
g2.

```c
#include <stdio.h>
#include <g2.h>
#include <g2_X11.h>
#define YELLOW 25
#define BLACK 1
int main() {
    int dev = g2_open_X11(200, 200);
    g2_set_background(dev, BLACK);
    g2_pen(dev, YELLOW);
    g2_filled_triangle(dev, 100, 10, 10, 190, 190, 190);
    getchar();
    g2_close(dev);
    return 0;
}
```

*Nota: Podes carregar figuras não vetoriais para o GitHub criando um novo
[issue](https://github.com/VideojogosLusofona/ic_exercicios/issues) e
arrastando a figura para o local onde é suposto escreveres o comentário. Isto
cria um _link_ que podes colocar na solução.*

> [Soluções](../solucoes/19_bib_g2/02.md)

3 - Escreve um programa em C que peça ao utilizador a dimensão de uma imagem
(_x_ e _y_), bem como _n_ pontos de um polígono. O programa deve depois criar
um ficheiro PNG com a dimensão especificada pelo utilizador, com fundo azul e
com um polígono preenchido de vermelho, criado a partir dos _n_ pontos
indicados pelo utilizador.

> [Soluções](../solucoes/19_bib_g2/03.md)
