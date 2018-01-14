# Gestão dinâmica da memória

1 - Escreve um programa em C que: 1) peça um valor _n_ (inteiro) ao utilizador;
2) peça _n_ valores reais ao utilizador; e finalmente, 3) calcule a média e a
mediana dos _n_ valores reais inseridos pelo utilizador. Deves usar alocação
dinâmica de memória. Não te esqueças de libertar a memória alocada.

> [Soluções](../solucoes/15_mem/01.md)

2 - Completa a seguinte função, que recebe um array de _doubles_ e um inteiro
com indicação do tamanho desse array. A função devolve um novo array, de
_shorts_, em que cada elemento é 1, -1 ou 0 caso o respetivo _double_ no array
recebido seja positivo, negativo ou zero. Neste caso a libertação da memória
alocada deve ser realizada por quem chamou a função, e não pela função em si.

```c
short *obter_sinal(double *array, int tamanho) {
    /* Inserir codigo aqui */
}
```

> [Soluções](../solucoes/15_mem/02.md)

3 - Implementa a tua própria versão da função `calloc()` chamada `my_calloc()`.
Podes usar a função `malloc()`.

```c
void *my_calloc(size_t num_elementos, size_t tamanho_de_cada_elemento) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```

> [Soluções](../solucoes/15_mem/03.md)

4 - Completa o código das funções `player_new()` e `player_destroy()`, que
inicializam e destroem um apontador para uma variável do tipo `PLAYER`,
respetivamente.

```c
/** Types of weapon. */
typedef enum { SWORD, DAGGER, AXE, MACE, PISTOL, MACHINEGUN, SHOTGUN,
    SNIPER_RIFLE, BFG9000, PLASMAGUN, NAILGUN, BBGUN, KNIFE, ROD, FLAMETHROWER,
    SLINGSHOT, SPEAR, LONGBOW, CROSSBOW, PIKE, GRENADE, MINE, GATLINGGUN,
    ASSAULT_RIFLE
} WEAPON;

/** Player structure. */
typedef struct {
    int id;           /**< Player ID.               */
    char *name;       /**< Player name.             */
    WEAPON *weapons;  /**< Array of player weapons. */
} PLAYER;

/**
 * @brief Create new player object.
 *
 * @param id The player ID.
 * @param name The player name. Must be copied to the player `name` field and
 * not be used directly.
 * @param num_weapons Number of weapons this player can hold at any given time.
 * @return A new player.
 * */
PLAYER *player_new(int id, char *name, int num_weapons) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}

/**
 * @brief Destroy a player object.
 *
 * @param player Player object to destroy.
 * */
void player_destroy(PLAYER *player) {
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```

> [Soluções](../solucoes/15_mem/04.md)

5 - Escreve um programa em C que faça uso das funções do problema anterior,
peça ao utilizador um valor _n_ (número de _players_), e para cada _player_
peça ao utilizador o nome e número de armas que esse _player_ pode carregar. O
ID de cada player é determinado automaticamente e começa em 1. As armas de cada
_player_ devem ser geradas aleatoriamente (sendo permitido que os mesmos tenham
armas repetidas). Os _players_ criados devem ser guardados num array de
apontadores para `PLAYER`, criado dinamicamente. O programa deve então mostrar
no ecrã o ID, nome e armas de todos os players. Toda a memória alocada deve ser
devidamente libertada antes do programa terminar.

> [Soluções](../solucoes/15_mem/05.md)

6 - Experimenta compilar e executar o seguinte programa. Porque razão o
programa termina com _segmentation fault_ ou aparece com valores esquisitos?
Qual a instrução necessária no lugar do comentário `/* (1) */` para evitar
estes problemas? Qual a instrução necessária no lugar do comentário `/* (2) */`
de modo a que o programa fique formalmente correto?

```c
#include <stdio.h>
#include <stdlib.h>
int main() {
    int *p;
    /* (1) */
    *p = 23;
    printf("Valor apontado por p = %d\n", *p);
    /* (2) */
    return 0;
}
```

> [Soluções](../solucoes/15_mem/06.md)
