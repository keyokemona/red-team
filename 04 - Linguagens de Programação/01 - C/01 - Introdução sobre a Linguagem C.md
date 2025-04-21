---
cards-deck: 04 - Linguagens de Programação::01 - C
---

# Variáveis
#card
As variáveis são locais de armazenamento em memória onde os dados podem ser armazenados e manipulados durante a execução de um programa.

Aqui está um exemplo de como declarar e atribuir um valor a uma variável em C:

```c
#include <stdio.h>

int main(void) {
	// Declara uma variável inteira chamada "idade"
	int idade;

	// Atribui o valor 25 à variável "idade"
	idade = 25;

	prinf("Minha idade é: %d\n", idade);

	return 0;
}
```

Neste exemplo, a variável "idade" é declarada como um inteiro. Ela é então atribuída o valor 25 através da atribuição de valor `idade = 25`. O valor da variável "idade" é então exibido na tela através da função `printf()`.

O resultado da execução deste programa seria: "Minha idade é: 25".

# Tipos de dados
#card 
A linguagem C possui vários tipos de dados, como **inteiros (`int`), ponto flutuante (`float`), strings/caracteres (`char`) e booleanos (`_Bool`)**.

Veja como usar diferentes tipos de dados em C:
```c
#include <stdio.h>

int main(void) {
	// Declara uma variável inteira chamada "idade" e atribui o valor 25
	int idade = 25;

	// Declara uma variável de ponto flutuante chamada "altura" e atribui o valor 1.80
	float altura = 1.80;

	// Declara uma variável de caractere chamada "sexo" e atribui o valor 'M'
	char sexo = 'M';

	// Declara uma variável booleana chamada "casado" e atribui o valor verdadeiro
	_Bool casado = 1;

	printf("Idade: %d\nAltura: %f\nSexo: %c\nCasado: %d\n", idade, altura, sexo, casado);

	return 0;
}
```

Neste exemplo, são declaradas quatro variáveis de diferentes tipo: inteiro, ponto flutuante, string (caractere) e booleano. Cada uma delas é atribuída um valor apropriado e, em seguida, é exibida na tela através da função `printf()`.

O resultado da execução deste programa seria:
![[Pasted image 20250420220204.png]]

> [!TIP] Diferença na declaração de variável `char` com ' (aspas simples) e " (aspas duplas)
> - O uso de aspas simples em uma variável de tipo `char` representa um único caractere, que é, por exemplo:
> ```c
> char nome[5] = 'Keyo' //  É o valor ASCII de 'K', 'e', 'y', 'o' combinados
> ```
> - Enquanto o uso de aspas duplas em uma variável de tipo `char` representa uma string, que é uma sequência de caracteres terminada com um caractere nulo `\0`, a qual é a forma correta de inicializar um array de caracteres (`char`) com uma string literal. Por exemplo:
> ```c
> char nome[5] = "Keyo" // Inicializa um array de `char` com uma string literal
> ```


**CONTINUAR EM:**
https://embarcados.com.br/linguagem-c-guia-completo/#Introducao-sobre-a-linguagem-C:~:text=execu%C3%A7%C3%A3o%20deste%20programa%3A-,Operadores%C2%A0,-Os%20operadores%20s%C3%A3o