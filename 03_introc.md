# Introdução ao C

Soluções disponíveis [aqui](03_introc_sol.md).

**1 - Indique pelo menos duas vantagens de aprender a linguagem de programação
C.**

**2 - Indente o seguinte programa em C num estilo legível e consistente.**

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

**3 - Indente o seguinte programa em C num estilo legível e consistente.**

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

**4 - Indente o seguinte programa em C num estilo legível e consistente.**

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

**5 - Indente o seguinte programa em C num estilo legível e consistente.**

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

**6 - Indique pelo menos duas práticas de programação em C.**

**7 - Indique quais dos seguintes nomes são válidos para variáveis e funções
em C:**

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

**8 - Indique duas formas de definir constantes em C.**

**9 - A _keyword_ `sizeof` é uma função ou um operador? Qual é a sua
funcionalidade?**

**10 - Como representar literais hexadecimais e octais em código C?**

**11 - Qual o carácter "escondido" com que terminam todas as strings?**

**12 - Qual dos seguintes tipos requer mais bits para ser representado?
`char` ou `int`?**

**13 - Qual dos seguintes tipos requer mais bits para ser representado?
`float` ou `double`?**

**14 - O que faz o operador `!`?**
