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
enum situacao sit_atual = 2;

enum situacao obter_situacao() {
    return sit_atual;
}

void definir_situacao(enum situacao sit) {
    sit_atual = sit;
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

3 - Qual é o problema em cada uma das seguintes declarações em C?

1. `struct ponto { float x, float y }`
2. `struct ponto { float x; float y }`
3. `struct ponto ( float x, y )`
4. `struct ponto { float x; float y; }`
5. `struct ponto { float x; float y; };`

> [Soluções](../solucoes/14_tipos/03.md)

4 - O que acontece quando passamos diretamente uma `struct` como argumento de
uma função?

1. É passado o endereço de memória da `struct` (passagem por referência)?
2. Ou, os valores dos campos da `struct` são copiados para uma nova `struct`
   dentro da função (passagem por valor)?

Caso a função altere os campos da `struct`, a `struct` original também é
modificada? Por outro lado, quando uma função retorna diretamente uma `struct`,
retorna a sua referência (endereço de memória) ou retorna o seu valor (isto é,
uma cópia)?

> [Soluções](../solucoes/14_tipos/04.md)

5 - Considera que tens o seguinte código:

```c
enum npc_race { ORCS, ELVES, DWARFS, SKAVEN, MEN, LIZARDMEN };
struct player { int id; char *name; int level; };
struct npc { int id; enum npc_race race; float power; };

struct player plyr = { 12, "The Red Duke", 23 };
struct npc nonplyr = { 57, ELVES, 99.34 };
struct npc *pnp = &nonplyr;
```

Escreve as instruções C para fazer o seguinte:

1. Mostrar no ecrã o ID e nome do _player_ guardado na variável `plyr`
2. Mostrar no ecrã o ID e o _power_ no NPC guardado na variável `nonplyr`
3. Mesma coisa que o ponto anterior, mas usando a variável `pnp`

> [Soluções](../solucoes/14_tipos/05.md)

<a name="p6" />

6 - Considera que tens a seguinte estrutura:

```c
struct fps_player { short health; short ammo; short armor; };
```

Completa o código da seguinte função, cujo objetivo é simplesmente preencher os
campos da estrutura passada como primeiro argumento com os valores passados no
2º, 3º e 4º argumentos.

```c
void preenche(struct fps_player *fplyr, short health, short ammo, short armor)
{
    /* ************ */
    /* Codigo aqui! */
    /* ************ */
}
```

> [Soluções](../solucoes/14_tipos/06.md)

## Definição de tipos

7 - Qual é o problema em cada uma das seguintes declarações em C?

1. `typedef { double x; double y; } PONTO;`
2. `typedef struct { double x; double y } PONTO;`
3. `typedef struct ponto { double x; double y; } PONTO;`
4. `typedef struct { double x; double y; };`
5. `typedef struct { double x; double y; } PONTO;`

> [Soluções](../solucoes/14_tipos/07.md)

8 - Qual é a diferença prática entre as seguintes declarações:

1.

```c
typedef struct ponto { double x; double y; } PONTO;
```

2.

```c
typedef struct { double x; double y; } PONTO;
```

3.

```c
struct ponto { double x; double y; };
typedef struct ponto PONTO;
```

4.

```c
typedef struct ponto PONTO;
struct ponto { double x; double y; };
```

> [Soluções](../solucoes/14_tipos/08.md)

9 - Reescreve o código da `struct fps_player` e da função `preenche`
([exercício 6](#p6)) de modo a que a estrutura em questão se passe a chamar
`FPS_PLAYER`.

> [Soluções](../solucoes/14_tipos/09.md)
