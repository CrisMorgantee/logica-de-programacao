---
icon: up-right-and-down-left-from-center
---

# Estruturas de Controle e Condicionais

## **Introdução às Estruturas Condicionais**

### **O que são Estruturas Condicionais?**

Estruturas condicionais permitem que o programa tome decisões com base em condições específicas. É como dizer ao computador: "Se isso acontecer, faça isso; caso contrário, faça outra coisa."

**O `if`, `else if`, e `else` em JavaScript**

* **`if`**: Executa o bloco de código se a condição for verdadeira.
* **`else if`**: Testa outra condição se a primeira não for verdadeira.
* **`else`**: Executa o bloco de código se nenhuma das condições anteriores for verdadeira.

**Exemplo Prático**:

```javascript
let idade = 18;

if (idade >= 18) {
    console.log("Você é maior de idade.");
} else {
    console.log("Você é menor de idade.");
}
```

**Explicação**:

* Aqui, o programa verifica se a idade é 18 ou mais.
* Se for, ele exibe "Você é maior de idade".
* Caso contrário, exibe "Você é menor de idade".
