---
icon: right-left-large
---

# Métodos Básicos de Arrays

## **Adicionar Elementos ao Array**

1. **`push`**: Adiciona um novo elemento ao final do array.
2. **`unshift`**: Adiciona um novo elemento ao início do array.

**Exemplo Prático**:

```javascript
let frutas = ["Maçã", "Banana"];
frutas.push("Laranja");
console.log(frutas); // Saída: ["Maçã", "Banana", "Laranja"]

frutas.unshift("Morango");
console.log(frutas); // Saída: ["Morango", "Maçã", "Banana", "Laranja"]
```

### **Remover Elementos do Array**

1. **`pop`**: Remove o último elemento do array.
2. **`shift`**: Remove o primeiro elemento do array.

**Exemplo Prático**:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];
frutas.pop();
console.log(frutas); // Saída: ["Maçã", "Banana"]

frutas.shift();
console.log(frutas); // Saída: ["Banana"]
```

### **Percorrendo um Array com Estruturas de Repetição**&#x20;

Muitas vezes, queremos realizar uma operação em cada elemento de um array. Podemos fazer isso usando uma estrutura de repetição `for` para percorrer o array.

**Exemplo Prático**:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];

for (let i = 0; i < frutas.length; i++) {
    console.log(frutas[i]);
}
```

**Explicação do Código**:

* `for (let i = 0; i < frutas.length; i++)`: Este loop percorre cada posição do array `frutas`.
* `frutas[i]`: Acessa o elemento atual no índice `i`.

**Saída**:

```
Maçã
Banana
Laranja
```
