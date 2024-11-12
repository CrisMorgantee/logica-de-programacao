---
icon: display-code
---

# Tarefa para Praticar

Crie um programa que avalie o desempenho de um aluno com base em uma nota fixa (de 0 a 100) e exiba uma mensagem de acordo com a pontuação.

**Regras de Avaliação**:

* **De 90 a 100**: "Excelente"
* **De 70 a 89**: "Bom"
* **De 50 a 69**: "Regular"
* **Abaixo de 50**: "Precisa Melhorar"

#### **Resposta:**

```javascript
// Definindo a nota do aluno
let nota = 85; // Modifique esse valor para testar diferentes avaliações

// Avaliando o desempenho com base na pontuação
if (nota >= 90 && nota <= 100) {
    console.log("Excelente");
} else if (nota >= 70 && nota < 90) {
    console.log("Bom");
} else if (nota >= 50 && nota < 70) {
    console.log("Regular");
} else if (nota >= 0 && nota < 50) {
    console.log("Precisa Melhorar");
} else {
    console.log("Nota inválida. Digite um valor entre 0 e 100.");
}
```

#### **Explicação do Código**

1. **Variável `nota`**: A variável `nota` armazena a pontuação do aluno. Para simular diferentes cenários, os alunos podem alterar o valor dessa variável.
2. **Estrutura Condicional `if-else`**:
   * O programa verifica a faixa de valor da variável `nota` e exibe a avaliação correspondente:
     * **90 a 100**: Exibe "Excelente"
     * **70 a 89**: Exibe "Bom"
     * **50 a 69**: Exibe "Regular"
     * **Abaixo de 50**: Exibe "Precisa Melhorar"
   * Se o valor de `nota` estiver fora do intervalo de 0 a 100, o programa exibe "Nota inválida".
