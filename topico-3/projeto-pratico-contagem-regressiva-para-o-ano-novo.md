---
icon: stopwatch-20
---

# Projeto Prático: Contagem Regressiva para o Ano Novo

## **Objetivo do Projeto**&#x20;

Criar um programa que conta de 10 até 1 e exibe uma mensagem de “Feliz Ano Novo!” ao final. Esse projeto vai usar a estrutura `for` para a contagem regressiva.

### **Passo a Passo**

**Passo 1**: Crie a estrutura `for` para começar a contagem de 10 e ir até 1.

```javascript
for (let i = 10; i >= 1; i--) {
    console.log("Contagem regressiva:", i);
}
```

**Passo 2**: Adicione a mensagem "Feliz Ano Novo!" ao final da contagem.

```javascript
for (let i = 10; i >= 1; i--) {
    console.log("Contagem regressiva:", i);
}

console.log("Feliz Ano Novo!");
```

**Código Completo**:

```javascript
for (let i = 10; i >= 1; i--) {
    console.log("Contagem regressiva:", i);
}

console.log("Feliz Ano Novo!");
```

**Explicação do Código**:

* O loop começa em 10 e termina em 1, com `i--` reduzindo o valor de `i` em 1 a cada repetição.
* Quando o loop termina, o programa exibe "Feliz Ano Novo!".

**Atividade Guiada**: Experimente outras contagens, como começar de 5 ou 20, para ver como pode personalizar o código.

**Tarefa para Praticar**

Crie um programa que exiba todos os números pares entre 1 e 20.
