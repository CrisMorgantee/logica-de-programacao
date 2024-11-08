---
icon: arrow-progress
---

# Métodos em Objetos

## **O que é um Método?**

Um método é uma função que pertence a um objeto. É uma ação que o objeto pode realizar. Um método é criado como uma propriedade do objeto, onde o valor é uma função.

**Exemplo de Objeto com Método**:

```javascript
let pessoa = {
    nome: "Carlos",
    idade: 25,
    cumprimentar: function() {
        console.log("Olá, meu nome é " + this.nome);
    }
};

// Chamando o método
pessoa.cumprimentar(); // Saída: Olá, meu nome é Carlos
```

**Explicação**:

* `cumprimentar` é um método que pertence ao objeto `pessoa`.
* `this.nome` refere-se à propriedade `nome` dentro do próprio objeto `pessoa`.

**Atividade Guiada**: Adicione um método `descrever` ao objeto `carro` que exiba uma frase descrevendo o carro, como "Este carro é um Toyota Corolla de 2020".
