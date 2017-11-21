# Introdução ao C

1 - Indique pelo menos duas vantagens de aprender a linguagem de programação C.

> Aguarda solução

2 - Indente o seguinte programa em C num estilo legível e consistente.

```
#include <stdio.h>
int main() { int number;
printf("Insere um inteiro: ");
scanf("%d", &number);
if(number % 2 == 0) { printf("%d e’ par.", number); }
else { printf("%d e’ impar.", number);
}
return 0;}
```

> Aguarda solução

3 - Indente o seguinte programa em C num estilo legível e consistente.

```
#include <stdio.h>
int main()
{ long n; int count = 0;
printf("Insere um inteiro: ");
scanf("%ld", &n);
while(n != 0) {
n /= 10; ++count; }
printf("N. digitos: %d", count); return 0;
}
```

> Aguarda solução

4 - Indente o seguinte programa em C num estilo legível e consistente.

```
#include <stdio.h>
int main() {
    const int n = 5;
int i, factorial = 1;
        for(i=1; i<=n; ++i)
{ factorial *= i; }
printf("Factorial de %d = %d\n", n, factorial);
    return 0;}
```

> Aguarda solução

5 - Indente o seguinte programa em C num estilo legível e consistente.

```
#include <stdio.h>
int main()
         {
    int number, i;
printf("Insere um inteiro positivo: ");  scanf("%d",&number);
    printf("Os factores de %d sao: ", number);
    for(i=1; i <= number; ++i)
 { if (number%i == 0)
 { printf("%d ",i); }
  }    return 0; }
```

> Aguarda solução

6 - Indique pelo menos duas práticas de programação em C.

> Aguarda solução

7 - Indique quais dos seguintes nomes são válidos para variáveis e funções
em C:

```
avatar
123var
var123
_umavar_
-x
x-
x_
_x
y5
5y
z"
z'
ç1
var!
valx
```

> Aguarda solução


8 - Indique duas formas de definir constantes em C.

> Aguarda solução

9 - A _keyword_ `sizeof` é uma função ou um operador? Qual é a sua
funcionalidade?

> Aguarda solução

10 - Como representar literais hexadecimais e octais em código C?

> Aguarda solução

11 - Qual o carácter "escondido" com que terminam todas as strings?

> Aguarda solução

12 - Qual dos seguintes tipos requer mais bits para ser representado?
`char` ou `int`?

> Aguarda solução

13 - Qual dos seguintes tipos requer mais bits para ser representado?
`float` ou `double`?

> Aguarda solução

14 - O que faz o operador `!`?

> Aguarda solução
