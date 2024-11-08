---
icon: square-js
---

# Conceitos Básicos de JavaScript

### **Variáveis**

Em programação, variáveis são usadas para armazenar informações. Pense em variáveis como "caixinhas" onde armazenamos valores, como números, textos ou outros dados. Em JavaScript, podemos criar variáveis usando `let` ou `const`.&#x20;

* **`let`**: Usado para criar uma variável que pode mudar de valor.
* **`const`**: Usado para criar uma variável que não muda de valor.

**Exemplo Prático:**

```javascript
let nome = "Ana"; // Variável que armazena um texto (string)
let idade = 25;   // Variável que armazena um número (number)
const cidade = "São Paulo"; // Uma constante que não muda
```

Aqui, `nome` e `idade` são variáveis que podem mudar, enquanto `cidade` é uma constante e seu valor não pode ser alterado.

&#x20;Vou deixar um link abaixo para explicar com mais detalhes a questão de criação de variáveis pois existem alguns detalhes importantes para que você não se surpreender com algum comportamento inesperado no seu código.

Existem outras formas mais antigas que ja não são recomendadas utilizar para criação de variáveis por alguns motivos, como problemas de escopo por exemplo, você pode saber mais sobre as diferenças [aqui](https://cristianomorgante.netlify.app/variaveis-javascript-temporal-dead-zone/).

***

### **Tipos de Dados**

Em programação, cada valor tem um tipo de dado, que indica o tipo de informação que ele representa. Os principais tipos de dados em JavaScript são:

* **`String`**: Sequência de caracteres, como textos. Exemplo: `"Olá"`.
* **`Number`**: Números, incluindo inteiros e decimais. Exemplo: `25`, `3.14`.
* **`Boolean`**: Representa verdadeiro (`true`) ou falso (`false`).

**Exemplo Prático:**

```javascript
let nome = "Carlos";  // Tipo String
let idade = 30;       // Tipo Number
let isEstudante = true; // Tipo Boolean
```

***

