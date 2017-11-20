# Introdução ao C

**Indique pelo menos duas vantagens de aprender a linguagem de programação C.**

Resposta

**Indente o seguinte programa em C num estilo legível e consistente.**

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


Resposta

**Indente o seguinte programa em C num estilo legível e consistente.**

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


Resposta

**Indente o seguinte programa em C num estilo legível e consistente.**

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


Resposta

**Indente o seguinte programa em C num estilo legível e consistente.**

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

Resposta
