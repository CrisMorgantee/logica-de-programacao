---
icon: brain-arrow-curved-right
---

# Métodos Avançados de Manipulação de Arrays

### **Método `map`**

&#x20;`map` permite criar um novo array ao aplicar uma função a cada elemento do array original. Muito útil para transformar dados.

**Exemplo Prático**:

```javascript
let numeros = [1, 2, 3, 4];
let dobrados = numeros.map(num => num * 2);

console.log(dobrados); // [2, 4, 6, 8]
```

### **Método `filter`**

&#x20;`filter` cria um novo array contendo apenas os elementos que atendem a uma condição específica.

**Exemplo Prático**:

```javascript
let numeros = [1, 2, 3, 4, 5, 6];
let pares = numeros.filter(num => num % 2 === 0);

console.log(pares); // [2, 4, 6]
```

### **Método `reduce`**

&#x20;`reduce` reduz todos os elementos de um array a um único valor, acumulando o resultado ao longo do array.

**Exemplo Prático**:

```javascript
let numeros = [1, 2, 3, 4];
let soma = numeros.reduce((total, num) => total + num, 0);

console.log(soma); // 10
```

**Atividade Guiada**: Crie um array com números e, usando `map`, `filter`, e `reduce`, crie um array com todos os números multiplicados por 3, filtre os números pares, e some o total.

**Resposta:**

```javascript
// Array inicial com alguns números
let numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Passo 1: Multiplicar todos os números por 3 usando map
let multiplicadosPor3 = numeros.map(numero => numero * 3);
console.log("Multiplicados por 3:", multiplicadosPor3); 
// Saída: [3, 6, 9, 12, 15, 18, 21, 24, 27, 30]

// Passo 2: Filtrar apenas os números pares usando filter
let numerosPares = multiplicadosPor3.filter(numero => numero % 2 === 0);
console.log("Números Pares:", numerosPares); 
// Saída: [6, 12, 18, 24, 30]

// Passo 3: Somar todos os números pares usando reduce
let somaTotal = numerosPares.reduce((acumulador, numero) => acumulador + numero, 0);
console.log("Soma dos Números Pares:", somaTotal); 
// Saída: 90
```

#### **Explicação de Cada Passo**

**`map`**:

* `numeros.map(numero => numero * 3)` cria um novo array onde cada elemento de `numeros` é multiplicado por 3.
* **Resultado**: `[3, 6, 9, 12, 15, 18, 21, 24, 27, 30]`

**`filter`**:

* `multiplicadosPor3.filter(numero => numero % 2 === 0)` cria um novo array contendo apenas os números pares do array `multiplicadosPor3`.
* **Resultado**: `[6, 12, 18, 24, 30]`

**`reduce`**:

* `numerosPares.reduce((acumulador, numero) => acumulador + numero, 0)` calcula a soma de todos os elementos de `numerosPares`. O `0` no final é o valor inicial do acumulador.
* **Resultado**: `90`
