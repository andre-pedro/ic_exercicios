# Ficheiros

1 - Descreve por palavras tuas o que faz o seguinte programa. Opcionalmente
insere comentários no programa seguindo as melhores práticas (não ultrapassar
80 linhas, precedendo o código a que se referem, devidamente indentados com o
código, e usando apenas caracteres da Língua Inglesa):

```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {

    FILE *fp = NULL;
    char *filename = NULL;

    if (argc >= 2) {
        filename = argv[1];
    } else {
        filename = "default.txt";
    }

    fp = fopen(filename, "a");
    if (fp == NULL) {
        fprintf(stderr,
            "Nao foi possivel abrir ficheiro '%s'.\n",
            filename);
        exit(1);
    }

    fprintf(fp, "Era uma vez...\n");

    fclose(fp);

    return 0;
}
```

> [Soluções](../solucoes/13_ficheiros/01.md)

2 - Descreve por palavras tuas o que faz o seguinte programa. Opcionalmente
insere comentários no programa seguindo as melhores práticas (não ultrapassar
80 linhas, precedendo o código a que se referem, devidamente indentados com o
código, e usando apenas caracteres da Língua Inglesa):

```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {

    FILE *fp = NULL;

    fp = fopen("output.txt", "w");
    if (fp == NULL) {
        fprintf(stderr, "Nao foi possivel abrir ficheiro '%s'.\n", argv[1]);
        exit(1);
    }

    for (int i = 0; i < argc; ++i) {
        fprintf(fp, "%s\n", argv[i]);
    }
    fclose(fp);

    return 0;
}
```

> [Soluções](../solucoes/13_ficheiros/02.md)

3 - Descreve por palavras tuas o que faz o seguinte programa. Opcionalmente
insere comentários no programa seguindo as melhores práticas (não ultrapassar
80 linhas, precedendo o código a que se referem, devidamente indentados com o
código, e usando apenas caracteres da Língua Inglesa):

```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]) {

    FILE *fp = NULL;
    int contagem = 0;
    char c;

    if (argc >= 2) {
        fp = fopen(argv[1], "r");
        if (fp == NULL) {
            fprintf(stderr, "Nao foi possivel abrir ficheiro '%s'.\n", argv[1]);
            exit(1);
        }
        while ((c = fgetc(fp)) != EOF) {
            if (c == ' ') {
                contagem++;
            }
        }
        fclose(fp);
    }
    else {
        fprintf(stderr, "Por favor indique o nome do ficheiro a abrir.\n");
        exit(1);
    }

    printf("Contagem final: %d\n", contagem);

    return 0;
}
```

> [Soluções](../solucoes/13_ficheiros/03.md)

4 - Descreve por palavras tuas o que faz o seguinte programa. Opcionalmente
insere comentários no programa seguindo as melhores práticas (não ultrapassar
80 linhas, precedendo o código a que se referem, devidamente indentados com o
código, e usando apenas caracteres da Língua Inglesa):

```c
#include <stdio.h>
#include <stdlib.h>
#define MAXLINHA 500

int main(int argc, char *argv[]) {

    FILE *fp = NULL;
    char linha[MAXLINHA];

    if (argc >= 2) {
        fp = fopen(argv[1], "r");
        if (fp == NULL) {
            fprintf(stderr, "Nao foi possivel abrir ficheiro '%s'.\n", argv[1]);
            exit(1);
        }
        while (fgets(linha, MAXLINHA, fp) != NULL) {
            for (int i = 0; linha[i] != '\0'; ++i) {
                printf("%d ", linha[i]);
            }
            printf("\n");
        }
        fclose(fp);
    }
    else {
        fprintf(stderr, "Por favor indique o nome do ficheiro a abrir.\n");
        exit(1);
    }

    return 0;
}
```

> [Soluções](../solucoes/13_ficheiros/04.md)

5 - Escreve um programa em C para guardar, num ficheiro chamado "ascii.txt", o
valor ASCII em hexadecimal de cada um dos caracteres dos argumentos passados na
linha de comandos. Deve haver um espaço entre cada valor ASCII. Cada argumento
deve estar numa linha consecutiva do ficheiro. Por exemplo, se o programa for
chamado com os argumentos "ola adeus", os conteúdos do ficheiro "ascii.txt"
devem ser:

```
4f 6c 61
41 64 65 75 73
```

> [Soluções](../solucoes/13_ficheiros/05.md)
