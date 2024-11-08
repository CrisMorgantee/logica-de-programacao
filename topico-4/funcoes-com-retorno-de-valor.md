---
icon: inbox-out
---

# Funções com Retorno de Valor

## **O que é o Retorno de uma Função?**

O `return` em uma função permite que ela envie um valor de volta para quem chamou essa função. Em vez de apenas executar o código, a função pode devolver um valor que pode ser usado em outras partes do programa.

**Exemplo de Função com Retorno**:

```javascript
function soma(a, b) {
    return a + b;
}

let resultado = soma(3, 5);
console.log("Resultado:", resultado); // Saída: Resultado: 8
```

**Explicação**:

* `return a + b;` faz com que a função `soma` devolva o resultado da soma de `a` e `b`.
* Quando chamamos `soma(3, 5)`, o valor `8` é retornado e armazenado na variável `resultado`.

**Atividade Guiada**: Crie uma função chamada `multiplicacao` que receba dois números como parâmetros e retorne o resultado da multiplicação. Eles devem armazenar o valor retornado em uma variável e exibi-lo no console.
