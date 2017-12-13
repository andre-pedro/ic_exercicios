# Operações e operadores

1 - Que operacao aritmética é realizada com um _shift left_ de 1? Justifica a
tua resposta.

> [Soluções](../solucoes/05_operacoes/01.md)

2 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.

```c
int x;
x = 3 + 4.9;
```

> [Soluções](../solucoes/05_operacoes/02.md)

3 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.

```c
int x;
x = 3.1 + 4.9;
```

> [Soluções](../solucoes/05_operacoes/03.md)

4 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.

```c
unsigned char x;
x = -2;
```

> [Soluções](../solucoes/05_operacoes/04.md)

5 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.

```c
double x;
x = ((int) 5.75) + 10;
```

> [Soluções](../solucoes/05_operacoes/05.md)

6 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.

```c
short x = 2;
x *= 2.8;
```

> [Soluções](../solucoes/05_operacoes/06.md)

7 - Qual o valor de `x` e `y` após as seguintes instruções? Justifica a tua
resposta.

```c
char y = 2.3;
short x = -10;
x /= y--;
```

> [Soluções](../solucoes/05_operacoes/07.md)

8 - Qual o valor de `x` e `y` após as seguintes instruções? Justifica a tua
resposta.

```c
char y = 3;
short x = 9.6;
x %= --y;
```

> [Soluções](../solucoes/05_operacoes/08.md)

9 - Aplique a operação _shift left_ 3 (`<< 3`) ao valor 0xA9 (_unsigned_
8-bits) e indique o resultado em decimal. mostra todos os passos.

> [Soluções](../solucoes/05_operacoes/09.md)

10 - Aplique a operação shift right 2 (`>> 2`) ao valor 0xF4 (_unsigned_
8-bits) e indique o resultado em decimal. mostra todos os passos.

> [Soluções](../solucoes/05_operacoes/10.md)

11 - Qual o resultado em decimal da operação XOR (`^`) entre os valores 0xD3
e 0xF0 (_unsigneds_ de 8-bits)? mostra todos os passos.

> [Soluções](../solucoes/05_operacoes/11.md)

12 - Assume que a variável `x` tem o valor 0x3B (_unsigned_ de 8-bits). Qual
o resultado, em decimal, da seguinte operação (mostra todos os passos):
`~x & 0x12`.

> [Soluções](../solucoes/05_operacoes/12.md)

13 - Assume que a variável `x` tem o valor 0xD3 (_unsigned_ de 8-bits). Qual
o resultado, em octal, da seguinte operação (mostra todos os passos):
`x | 0x44`.

> [Soluções](../solucoes/05_operacoes/13.md)

14 - Assumindo que `x` tem o valor 3 e `y` o valor 4, qual o resultado da
seguinte operação (mostra todos os passos):
`(x > y) || !(y <= 10)`

> [Soluções](../solucoes/05_operacoes/14.md)

15 - Assumindo que `x` tem o valor 3 e `y` o valor 4, qual o resultado da
seguinte operação (mostra todos os passos):
`((x | y) > 5) || ((x & ~y) < 3)`

> [Soluções](../solucoes/05_operacoes/15.md)

16 - Assumindo que `x` tem o valor -5 e `y` o valor 5, e que ambas as variáveis
são do tipo `char`, qual o resultado da seguinte operação (mostra todos os passos):
`((x ^ y) < 0xF) && !(x == y))`

> [Soluções](../solucoes/05_operacoes/16.md)

17 - Assumindo que `x` tem o valor -2 e `y` o valor 7, qual o resultado da
seguinte operação (mostra todos os passos):
`x >= y ? ~x : ~y`

> [Soluções](../solucoes/05_operacoes/17.md)
