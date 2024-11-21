---
icon: brain-circuit
---

# Consolidando o Conhecimento de Funções e Parâmetros

## **O que é uma Função?**

Função é um bloco de código que executa uma tarefa específica. Ela pode ter parâmetros (dados de entrada) e retornar um valor.

**Exemplo Simples**: Função para somar dois números.

```javascript
function oi() {
    console.log('Oi, a função foi executada!')
}

console.log(oi()); // Saída: Oi, a função foi executada!
```

### **Funções com Parâmetros e Retorno**

**Revisão**: Explique novamente a importância dos parâmetros e do `return`. Os parâmetros permitem que a função trabalhe com valores diferentes cada vez que é chamada, enquanto o `return` envia o resultado de volta para quem chamou a função.

**Exemplo Prático**:

```javascript
function saudacao(nome) {
    return "Olá, " + nome + "!";
}

console.log(saudacao("Ana")); // Saída: "Olá, Ana!"
```
