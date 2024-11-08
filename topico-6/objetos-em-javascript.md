---
icon: brackets-curly
---

# Objetos em JavaScript

## Introdução ao Conceito de Objetos

### O que é um Objeto?

Um objeto é uma estrutura de dados que permite armazenar dados e funcionalidades relacionadas. Diferente dos arrays, que são usados para listas de valores, objetos são ideais para representar entidades complexas com várias características (ou propriedades).

Imagine que você quer representar uma “Pessoa”. Ela tem várias características, como nome, idade, e altura. Em um objeto, você pode armazenar todas essas informações juntas.

**Estrutura de um Objeto em JavaScript**

* Um objeto é criado usando `{ }` (chaves) e tem **propriedades** no formato `chave: valor`.

**Exemplo de Objeto**:

```javascript
let pessoa = {
    nome: "Carlos",
    idade: 25,
    altura: 1.75
};
```

**Explicação**:

* Aqui, `pessoa` é um objeto com três propriedades: `nome`, `idade` e `altura`.
* Cada propriedade tem um nome (`chave`) e um valor associado.
