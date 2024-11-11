---
icon: display-code
---

# Tarefa para Praticar

Crie um programa que pergunte ao usuário um número entre 1 e 100 e verifique se o número é "baixo" ou "alto".

#### **Resposta:**

&#x20;Para verificar se o número fornecido pelo usuário está abaixo ou acima de 50, podemos usar uma estrutura condicional simples (`if` e `else`). No exemplo abaixo, usamos valores fixos para `numero` para simplificar, já que o código está sendo executado no terminal sem um prompt interativo:

```javascript
let numero = 70; // Substitua pelo valor desejado entre 1 e 100

if (numero < 50) {
    console.log("O número é baixo.");
} else if (numero >= 50) {
    console.log("O número é alto.");
}
```

**Explicação**:

Se `numero` for menor que 50, o programa exibirá `"O número é baixo."`

Se `numero` for 50 ou mais, o programa exibirá `"O número é alto."`

**Observação**: Esse código é escrito para Node.js sem entrada de usuário interativa. Para capturar entradas de forma interativa, podemos implementar o `readline`, mas neste caso estamos simplificando para focar na lógica da condição.
