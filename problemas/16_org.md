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
