---
icon: function
---

# Funções com Parâmetros

## **O que são Parâmetros?**

Parâmetros são valores que passamos para uma função para que ela possa usá-los em suas operações. Eles tornam as funções mais flexíveis, pois permitem que a função receba diferentes valores.

**Exemplo de Função com Parâmetros**:

```javascript
function saudacao(nome) {
    console.log("Olá, " + nome + "!");
}

// Chamando a função com um parâmetro
saudacao("Ana"); // Saída: Olá, Ana!
saudacao("Carlos"); // Saída: Olá, Carlos!
```

**Explicação**:

* Aqui, `nome` é um parâmetro da função `saudacao`.
* Quando chamamos `saudacao("Ana")`, o valor `"Ana"` é passado para o parâmetro `nome`, e a função exibe "Olá, Ana!".
* Isso permite que a função funcione para qualquer nome que passarmos.

**Atividade Guiada**: Crie uma função `saudacaoPersonalizada` que recebe dois parâmetros, `nome` e `idade`, e exibe uma mensagem como "Olá, João! Você tem 25 anos."
