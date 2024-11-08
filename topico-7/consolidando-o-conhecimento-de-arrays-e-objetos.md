---
icon: brain-circuit
---

# Consolidando o Conhecimento de Arrays e Objetos

### **Revisão de Arrays**

* **Definição**: Arrays são listas de valores armazenadas em uma única variável.
* **Métodos Básicos**: `push`, `pop`, `shift`, e `unshift`.
*   **Exemplo Prático**:

    ```javascript
    let frutas = ["Maçã", "Banana"];

    frutas.push("Laranja");
    frutas.unshift("Morango");

    console.log(frutas); // ["Morango", "Maçã", "Banana", "Laranja"]

    frutas.pop();
    frutas.shift();

    console.log(frutas); // ["Maçã", "Banana"]
    ```

### **Revisão de Objetos**

* **Definição**: Objetos permitem armazenar propriedades e métodos relacionados em uma única estrutura.
* **Modificação de Propriedades**: Adicionar, acessar e modificar propriedades de um objeto.
*   **Exemplo Prático**:

    ```javascript
    let aluno = {
        nome: "Carlos",
        idade: 18,
        notas: [7.5, 8.0, 9.0]
    };

    aluno.cidade = "São Paulo"; // Adicionando nova propriedade
    aluno.idade = 19; // Modificando propriedade existente

    console.log(aluno); // {nome: "Carlos", idade: 19, notas: [7.5, 8.0, 9.0], cidade: "São Paulo"}
    ```

