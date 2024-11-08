---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 💻 Introdução à Lógica de Programação e Algoritmos com JavaScript

### **O que é Programação?**

Programação é o processo de escrever instruções para que o computador execute tarefas. Sabemos que o computador é uma máquina muito eficiente, entretanto precisa receber instruções muito específicas para realizar qualquer ação. Programar é criar essas instruções de forma que o computador consiga entendê-las e executá-las.

Imagine que você quer que o computador diga "Olá, Mundo!". Você precisa instruir o computador exatamente para fazer isso. Em JavaScript, podemos escrever o seguinte código:

```javascript
console.log("Olá, Mundo!");
```

Aqui, `console.log()` é um comando que instrui o computador a mostrar uma mensagem na tela. Quando executamos este código, o computador lê as instruções e exibe a mensagem "Olá, Mundo!" no terminal ou na tela.

***

### **O que é um Algoritmo?**

Um algoritmo é uma sequência de passos para resolver um problema ou realizar uma tarefa. Você pode pensar em um algoritmo como uma receita de cozinha: ele define, passo a passo, o que precisa ser feito para alcançar um objetivo específico.

Vamos criar um "algoritmo" para fazer um café. Aqui estão os passos:

1. Ferva a água.
2. Coloque o pó de café no filtro.
3. Despeje a água quente sobre o pó.
4. Espere a água passar pelo filtro.
5. O café está pronto.

Esses passos formam um algoritmo. Quando estamos programando, criamos algoritmos para o computador seguir. Um exemplo simples de algoritmo em programação é somar dois números:

```javascript
let numero1 = 5;
let numero2 = 3;
let soma = numero1 + numero2;

console.log(soma); // Saída: 8
```

Neste código, temos uma sequência de passos (ou seja, um algoritmo) para somar dois números e mostrar o resultado.

***

### **O que é Lógica de Programação?**

Lógica de programação é a habilidade de resolver problemas de forma estruturada e organizada, usando passos lógicos e sequenciais. Em programação, é importante pensar nos passos que precisamos para resolver um problema, garantindo que cada etapa faça sentido e esteja na ordem correta.

Imagine que queremos criar um algoritmo para saber se uma pessoa é maior de idade ou não. Precisamos de uma estrutura lógica para isso:

1. Obtenha a idade da pessoa.
2. Se a idade for 18 ou mais, então ela é maior de idade.
3. Caso contrário, ela é menor de idade.

Aqui está o código em JavaScript para esse algoritmo:

```javascript
let idade = 20;
if (idade >= 18) {
    console.log("Você é maior de idade.");
} else {
    console.log("Você é menor de idade.");
}
```

Nesse exemplo, usamos a lógica para fazer uma verificação condicional com `if` (se) e `else` (caso contrário).

