---
icon: greater-than-equal
---

# Operadores de Comparação e Lógicos

## Operadores de Comparação

&#x20;Os operadores de comparação permitem comparar valores e são usados nas condições do `if`.

### **Operadores Básicos**

Operadores são símbolos usados para realizar operações com variáveis. Os operadores mais comuns são os aritméticos e os de atribuição.

#### **Operadores Aritméticos**: `+` (adição), `-` (subtração), `*` (multiplicação), `/` (divisão),  `%` (resto da divisão).

```javascript
let a = 10;
let b = 5;

console.log(a + b); // Saída: 15 (soma)
console.log(a - b); // Saída: 5 (subtração)
console.log(a * b); // Saída: 50 (multiplicação)
console.log(a / b); // Saída: 2 (divisão)
```

#### **Operador de Atribuição**: `=` (usado para atribuir um valor a uma variável).

#### **Atribuição de adição: `+=`** Adiciona um valor à variável.

#### **Atribuição de subtração: `-=`** Subtrai um valor da variável.

#### **Outros incluem** **`*=`**, **`/=`**, **`%=`** para multiplicação, divisão e resto, respectivamente.

```javascript
let x = 10;
x += 5; // x agora é 15
x -= 2; // x agora é 13

//Atribuição de Multiplicação (*=):
let a = 5;
a *= 3; // Equivalente a a = a * 3; a agora é 15

//Atribuição de Divisão (/=):
let b = 10;
b /= 2; // Equivalente a b = b / 2; b agora é 5

//Atribuição de Resto (%=):
let c = 28;
c %= 5; // Equivalente a c = c % 5; c agora é 3

//Atribuição de Exponenciação (**=):
let d = 4;
d **= 2; // Equivalente a d = d ** 2; d agora é 16
```

#### **Operador de Comparação: `==`**, **`!=`**, **`===`**, **`!==`**, **`>`**, **`<`**, **`>=`**, **`<=`**

Permitem comparar valores.

* **Igual a (==):** Verifica igualdade de valor, mas não de tipo.
* **Estritamente igual a (===):** Verifica igualdade de valor e tipo.
* **Não igual (!=):** Verifica se os valores não são iguais.
* **Estritamente não igual (!==):** Verifica se os valores e tipos não são iguais.
* **Maior que (>), Menor que (<), Maior ou igual a (>=), Menor ou igual a (<=):** Compara valores numéricos.

```javascript
let igual = 5 == "5"; // true
let estritamenteIgual = 5 === "5"; // false
let maiorQue = 10 > 5; // true
let menorOuIgual = 5 <= 5; // true
```

**Exemplo Prático**:

```javascript
let nota = 8;

if (nota >= 7) {
    console.log("Aprovado");
} else {
    console.log("Reprovado");
}
```

Neste exemplo, se a nota for maior ou igual a 7, o programa exibe "Aprovado"; caso contrário, exibe "Reprovado".

### **Operadores Lógicos**

&#x20;Os operadores lógicos combinam várias condições. Os principais operadores lógicos são:

* **`&&`** (E): Verdadeiro se ambas as condições forem verdadeiras.
* **`||`** (OU): Verdadeiro se pelo menos uma das condições for verdadeira.
* **`!`** (NÃO): Inverte o valor de uma condição.

**Exemplo Prático**:

```javascript
let idade = 20;
let possuiCarteira = true;

if (idade >= 18 && possuiCarteira) {
    console.log("Pode dirigir");
} else {
    console.log("Não pode dirigir");
}
```

**Explicação**:

* Aqui, o programa verifica se a idade é maior ou igual a 18 **e** se a pessoa possui carteira de motorista.
* Ambos precisam ser verdadeiros para que a pessoa possa dirigir.
