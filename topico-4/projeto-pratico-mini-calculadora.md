---
icon: calculator
---

# Projeto Prático: Mini Calculadora

## **Objetivo do Projeto**

Criar uma mini calculadora que execute operações de adição, subtração, multiplicação e divisão, usando funções para cada operação.

### **Passo a Passo**

**Passo 1**: Crie quatro funções - `adicao`, `subtracao`, `multiplicacao` e `divisao`. Cada uma deve receber dois números como parâmetros e retornar o resultado da operação.

```javascript
function adicao(a, b) {
    return a + b;
}

function subtracao(a, b) {
    return a - b;
}

function multiplicacao(a, b) {
    return a * b;
}

function divisao(a, b) {
    return a / b;
}
```

**Passo 2**: Solicite que o usuário escolha a operação e forneça os números.

**Passo 3**: Use as funções de operação para calcular o resultado e exibi-lo.

**Código Completo**:

```javascript
function adicao(a, b) {
    return a + b;
}

function subtracao(a, b) {
    return a - b;
}

function multiplicacao(a, b) {
    return a * b;
}

function divisao(a, b) {
    if (b === 0) {
        return "Erro: Divisão por zero não é permitida.";
    }
    return a / b;
}

let numero1 = 10;
let numero2 = 5;

console.log("Adição:", adicao(numero1, numero2)); // 15
console.log("Subtração:", subtracao(numero1, numero2)); // 5
console.log("Multiplicação:", multiplicacao(numero1, numero2)); // 50
console.log("Divisão:", divisao(numero1, numero2)); // 2
```

**Explicação do Projeto**:

* Cada operação (adição, subtração, multiplicação e divisão) é uma função separada, permitindo que o código fique organizado e fácil de entender.
* A função `divisao` tem uma verificação adicional para evitar a divisão por zero, que é uma operação inválida.

**Atividade Guiada**: Adicione uma nova operação chamada `potencia`, que calcula o primeiro número elevado ao segundo número.&#x20;

#### **Resposta:**&#x20;

```javascript
// Função para a operação de potência
function potencia(a, b) {
    return a ** b;
}

// Valores de exemplo para os cálculos
let numero1 = 2;
let numero2 = 3;

// Chamada da função e exibição dos resultados
console.log("Potência:", potencia(numero1, numero2)); // Saída: 8
```

#### **Explicação da Função `potencia`**

* A função `potencia` recebe dois parâmetros, `a` e `b`, e retorna o resultado de `a` elevado a `b` usando o operador `**`.
* No exemplo acima, `potencia(2, 3)` calcula `2 ** 3`, que resulta em `8`.

Com essa nova função, a calculadora agora realiza operações de adição, subtração, multiplicação, divisão e potência. Essa atividade ajuda a reforçar o conceito de funções e o uso de parâmetros para realizar operações específicas.
