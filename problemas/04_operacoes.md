# Operações e operadores

Soluções disponíveis [aqui](04_operacoes_sol.md).

## Operações aritméticas

**1 - Que operacao aritmética é realizada com um _shift left_ de 1? Justifica a
tua resposta.**

**2 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.**

```c
int x;
x = 3 + 4.9;
```

**3 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.**

```c
int x;
x = 3.1 + 4.9;
```

**4 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.**

```c
unsigned char x;
x = -2;
```

**5 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.**

```c
double x;
x = ((int) 5.75) + 10;
```

**6 - Qual o valor de `x` após as seguintes instruções? Justifica a tua
resposta.**

```c
short x = 2;
x *= 2.8;
```

**7 - Qual o valor de `x` e `y` após as seguintes instruções? Justifica a tua
resposta.**

```c
char y = 2.3;
short x = -10;
x /= y--;
```

**8 - Qual o valor de `x` e `y` após as seguintes instruções? Justifica a tua
resposta.**

```c
char y = 3;
short x = 9.6;
x %= --y;
```

## Operações relacionais e lógicas

Em breve
Não esquecer ternário

## Operações bit a bit

**? - Aplique a operação _shift left_ 3 (`<< 3`) ao valor 0xA9 (_unsigned_
8-bits) e indique o resultado em decimal. Mostre todos os passos.**

**? - Aplique a operação shift right 2 (`>> 2`) ao valor 0xF4 (_unsigned_
8-bits) e indique o resultado em decimal. Mostre todos os passos.**

**? - Qual o resultado em decimal da operação XOR (`^`) entre os valores 0xD3
e 0xF0 (_unsigneds_ de 8-bits)? Mostre todos os passos.**

**? - Assuma que a variável `x` tem o valor 0x3B (_unsigned_ de 8-bits). Qual
o resultado, em decimal, da seguinte operação (mostre todos os passos):
`~x & 0x12`.**

**? - Assuma que a variável `x` tem o valor 0xD3 (_unsigned_ de 8-bits). Qual
o resultado, em octal, da seguinte operação (mostre todos os passos):
`x | 0x44`.**
