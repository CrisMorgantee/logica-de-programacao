---
icon: head-side-goggles
---

# Introdução às Funções de Ordem Superior (Higher-Order Function)

## Higher-Order Function

### **O que são Funções de Ordem Superior?**

&#x20;Funções de ordem superior são funções que recebem outras funções como parâmetros ou retornam funções. Isso permite criar comportamentos flexíveis e é muito útil para manipulação de dados em JavaScript.

**Exemplo Prático de Função de Ordem Superior: Aplicar uma operação a cada elemento de um array.**

```javascript
function aplicarOperacao(numeros, operacao) {
    return numeros.map(operacao);
}

let numeros = [1, 2, 3];
let dobrados = aplicarOperacao(numeros, num => num * 2);

console.log(dobrados); // Saída: [2, 4, 6]
```

**Exemplo com `filter` e Função de Ordem Superior**

Use `filter` para mostrar como é possível usar funções como argumentos de outras funções para realizar operações flexíveis.

```javascript
let numeros = [1, 2, 3, 4, 5, 6];
let pares = numeros.filter(num => num % 2 === 0);

console.log(pares); // Saída: [2, 4, 6]
```

**Atividade Guiada**: Peça aos alunos para criar uma função `filtrarImpares` que recebe um array e retorna apenas os números ímpares usando `filter`.

#### **Resposta:**

```javascript
// Função que filtra e retorna apenas os números ímpares
function filtrarImpares(array) {
    return array.filter(numero => numero % 2 !== 0);
}

// Exemplo de uso da função com um array de números
let numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let impares = filtrarImpares(numeros);

console.log("Números Ímpares:", impares);
// Saída: [1, 3, 5, 7, 9]
```

#### **Explicação da Função `filtrarImpares`**

1. **Parâmetro `array`**: A função `filtrarImpares` recebe um array de números como argumento.
2. **Método `filter`**: Utilizamos o método `filter` para criar um novo array contendo apenas os elementos que satisfazem a condição `numero % 2 !== 0` (ou seja, que têm resto 1 na divisão por 2).
3. **Retorno**: A função retorna um novo array com apenas os números ímpares do array original.

#### **Exemplo de Saída**

Se chamarmos `filtrarImpares([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])`, a saída será `[1, 3, 5, 7, 9]`, que são os números ímpares do array original.
