---
icon: rectangle-list
---

# Acessando e Modificando Elementos do Array

## **Acessando Elementos**

Podemos acessar elementos de um array usando seu índice (posição). Em JavaScript, os índices começam em 0, o que significa que o primeiro elemento está na posição 0, o segundo na posição 1, e assim por diante.

**Exemplo Prático**:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];

console.log(frutas[0]); // Saída: Maçã
console.log(frutas[1]); // Saída: Banana
console.log(frutas[2]); // Saída: Laranja
```

### **Modificando Elementos**

Podemos alterar um elemento do array acessando-o pelo índice e atribuindo um novo valor.

**Exemplo Prático**:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];
frutas[1] = "Uva";

console.log(frutas); // Saída: ["Maçã", "Uva", "Laranja"]
```
