# Strings

1 - Completa o código da seguinte função, cujo objectivo é converter todos os
espaços numa string em underscores. Por exemplo, a string "Bem vindo a Lisboa!"
seria transformada em "Bem_vindo_a_Lisboa". Não uses funções da biblioteca
`string.h`.

```c
void subst_espacos_por_underscores(char *string)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/01.md)

2 - Completa o código da seguinte função, cujo objectivo é contar o número de
caracteres existentes numa string (ou seja, determinar o comprimento da string).
Não uses funções da biblioteca `string.h`.

```c
int comprimento_string(char *string)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/02.md)

3 - Completa o código da seguinte função, cujo objectivo é comparar se duas
strings são iguais, independentemente de minúsculas e maiúsculas. Por exemplo,
a função deve devolver 1 (`TRUE`) para as strings "Ola" e "OLA", mas deve
devolver 0 (`FALSE`) para as strings "Ola" e "Ole". Não uses funções da
biblioteca `string.h`.

```c
int compara_strings_indep_maiusc(char *str1, char *str2)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/03.md)

4 - Completa o código da função `quantas_vezes`, cujo objectivo é devolver o
número de vezes que determinado carácter (dado pela variável `c`) ocorre numa
string. Por exemplo, a chamada `quantas_vezes("Universidade Lusofona", 'a')
deve devolver 2. Não uses funções da biblioteca `string.h`.

```c
int quantas_vezes(char *string, char c)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/04.md)

5 - Completa o código da função `inverte`, cujo objectivo é inverter a string
passada como argumento. Indica porque razão a string passada como argumento não
pode ser um literal string. Não uses funções da biblioteca `string.h`.

```c
void inverte(char *str)
{
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/05.md)

6 - Completa o código da seguinte função, cujo objectivo é devolver um
apontador para a 1ª ocorrência de determinado carácter (dado pela variável `c`)
numa string. Caso a string não contenha esse carácter, a função deve devolver
`NULL`. Não uses funções da biblioteca `string.h`.

```c
char *ocorrencia(char *string, char c) {
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/06.md)

7 - Escreve um programa em C que indique quantos argumentos passados na linha
comandos são números inteiros de base decimal (ou seja, compostos inteiramente
por dígitos de 0-9). Faz o mesmo para números inteiros de base octal e base
hexadecimal.

> [Soluções](../solucoes/12_strings/07.md)

8 - Escreve um programa em C que indique qual dos argumentos passados na linha
comandos tem o maior comprimento.

> [Soluções](../solucoes/12_strings/08.md)

9 - Completa o código da função `implode`, cujo objectivo é concatenar todas
as strings passadas no 1º argumento, usando a string passada no 2º argumento
como `cola`. O 1º argumento, chamado `arr_str`, é um array de strings, cujo
último valor é `NULL`, indicando o final do mesmo. Por exemplo, o seguinte
programa imprime no ecrã `Ola**Boa tarde**Adeus`:

```c
char *varias_strings[] = {"Ola", "Boa tarde", "Adeus", NULL};
char *juntas = implode(varias_strings, "**");
printf("%s", juntas);
```

Para resolver este problema é necessário o uso de alocação dinâmica de memória
e podem ser usadas funções da biblioteca `string.h`.

```c
char *implode(char *arr_str[], char *cola) {
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/09.md)


10 - Completa o código da função `explode`, cujo objectivo é separar todas
as strings passadas no 1º argumento usando o carácter passado no 2º argumento
como `separador`. A função deve devolver um array de strings, o último
componente do qual deve ser `NULL`. Por exemplo, se a função for chamada da
seguinte forma, `explode("Ola mundo !", " ");`, a mesma deve devolver um array
com os seguintes conteúdos: `"Ola"`, `"mundo"`, `"!"`, `NULL`.

Para resolver este problema é necessário o uso de alocação dinâmica de memória
e podem ser usadas funções da biblioteca `string.h`.

```c
char **explode(char *string, char separador) {
    /* Codigo aqui. */
}
```

> [Soluções](../solucoes/12_strings/10.md)
