---
icon: diagram-project
---

# Projeto Prático: Verificador de Idade e Categoria

## **Objetivo do Projeto**&#x20;

Criar um programa que peça ao usuário sua idade e diga se ele é criança, adolescente, adulto ou idoso, com base em faixas etárias específicas. Este projeto usa estruturas condicionais para categorizar a idade.

### **Passo a Passo**

**Passo 1:** Declare uma variável para armazenar a idade.

```javascript
let idade = 25; // Substitua pelo valor que deseja testar
```

**Passo 2:** Crie condições para verificar a faixa etária.

* **Criança**: Idade até 12 anos.
* **Adolescente**: Idade de 13 a 17 anos.
* **Adulto**: Idade de 18 a 64 anos.
* **Idoso**: Idade de 65 anos ou mais.

**Passo 3:** Use `if`, `else if`, e `else` para exibir a categoria correspondente.

```javascript
if (idade <= 12) {
    console.log("Você é uma criança.");
} else if (idade >= 13 && idade <= 17) {
    console.log("Você é um adolescente.");
} else if (idade >= 18 && idade <= 64) {
    console.log("Você é um adulto.");
} else {
    console.log("Você é um idoso.");
}
```

**Explicação do Código**:

O código usa uma série de condições para verificar a faixa etária da pessoa e exibir a mensagem correspondente.

O uso de `&&` (E) nas condições ajuda a definir o intervalo de idade para cada categoria.

**Código Completo**:

```javascript
let idade = 25;

if (idade <= 12) {
    console.log("Você é uma criança.");
} else if (idade >= 13 && idade <= 17) {
    console.log("Você é um adolescente.");
} else if (idade >= 18 && idade <= 64) {
    console.log("Você é um adulto.");
} else {
    console.log("Você é um idoso.");
}
```

**Exemplos para Explorar:**

1.  E se uma pessoa tiver exatamente 18 anos? Em qual categoria ela se enquadra?

    **Resposta:** Neste caso, uma pessoa com exatamente 18 anos cairia na terceira condição (`idade >= 18 && idade <= 64`), ou seja, ela seria classificada como **"adulto"**.
2.  Como você alteraria o código para adicionar uma categoria para bebês (0 a 2 anos)?

    **Resposta:**&#x20;

    Para incluir uma nova categoria de "bebês" para idades entre 0 e 2 anos, podemos adicionar uma nova condição `else if`no início da sequência, pois a verificação precisa ser feita antes das outras categorias.

    Aqui está o código atualizado:

    ```javascript
    if (idade >= 0 && idade <= 2) {
        console.log("Você é um bebê.");
    } else if (idade <= 12) {
        console.log("Você é uma criança.");
    } else if (idade >= 13 && idade <= 17) {
        console.log("Você é um adolescente.");
    } else if (idade >= 18 && idade <= 64) {
        console.log("Você é um adulto.");
    } else {
        console.log("Você é um idoso.");
    }
    ```



    Com essa alteração:

    * Idades entre **0 e 2 anos** serão categorizadas como "bebê".
      * As demais categorias permanecem inalteradas.

