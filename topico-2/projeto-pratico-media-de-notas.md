---
icon: calculator
---

# Projeto Prático: Média de Notas

## **Objetivo do Projeto**

Criar um programa que calcula a média de três notas e informa se o aluno foi aprovado (média maior ou igual a 7) ou reprovado.

### **Passo a Passo**

1.  **Declare Três Variáveis para as Notas**

    ```javascript
    let nota1 = 8.0;
    let nota2 = 7.5;
    let nota3 = 6.0;
    ```
2.  **Calcule a Média**

    * Para calcular a média, somamos as notas e dividimos pelo número de notas.

    ```javascript
    let media = (nota1 + nota2 + nota3) / 3;
    ```
3.  **Verifique se o Aluno foi Aprovado**

    * Se a média for maior ou igual a 7, o aluno está aprovado.

    ```javascript
    if (media >= 7) {
        console.log("Aprovado com média: " + media.toFixed(2));
    } else {
        console.log("Reprovado com média: " + media.toFixed(2));
    }
    ```

**Explicação Completa do Código:**

* `nota1`, `nota2`, `nota3`: Variáveis que armazenam as três notas do aluno.
* `media`: Variável que armazena a média calculada.
* O método `.toFixed(2)` em JavaScript é utilizado para formatar números decimais, limitando o número de casas decimais exibidas após a vírgula (ou ponto, no caso da notação anglo-saxônica).
  * **Arredondamento Automático**: O método `.toFixed()` também arredonda o número automaticamente. Por exemplo:
    * Se `media` for `7.335`, `media.toFixed(2)` resultará em `7.34` (arredondamento para cima).
    * Se `media` for `7.333`, `media.toFixed(2)` resultará em `7.33`.
* Condicional `if-else`: Verifica se a média é maior ou igual a 7 e exibe a mensagem apropriada. Veremos mais sobre condicionais adiante.
