---
icon: address-card
---

# Projeto Prático: Cadastro de Aluno

## **Objetivo do Projeto**&#x20;

Criar um objeto `aluno` que armazena dados de um estudante e inclui métodos para exibir as informações do aluno e calcular a média das notas.

### **Passo a Passo**

**Passo 1**: Crie o objeto `aluno` com as propriedades `nome`, `idade`, e `notas` (um array de três notas).

```javascript
let aluno = {
    nome: "Ana",
    idade: 17,
    notas: [8.5, 7.0, 9.2]
};
```

**Passo 2**: Adicione um método `exibirInformacoes` que exibe o nome e a idade do aluno.

```javascript
aluno.exibirInformacoes = function() {
    console.log("Nome: " + this.nome);
    console.log("Idade: " + this.idade);
};
```

**Passo 3**: Adicione um método `calcularMedia` que calcula e retorna a média das notas do aluno.

```javascript
aluno.calcularMedia = function() {
    let soma = 0;
    for (let i = 0; i < this.notas.length; i++) {
        soma += this.notas[i];
    }
    return soma / this.notas.length;
};
```

**Passo 4**: Chame os métodos `exibirInformacoes` e `calcularMedia` e exiba a média no console.

**Código Completo**:

```javascript
let aluno = {
    nome: "Ana",
    idade: 17,
    notas: [8.5, 7.0, 9.2],
    
    exibirInformacoes: function() {
        console.log("Nome: " + this.nome);
        console.log("Idade: " + this.idade);
    },

    calcularMedia: function() {
        let soma = 0;
        for (let i = 0; i < this.notas.length; i++) {
            soma += this.notas[i];
        }
        return soma / this.notas.length;
    }
};

// Chamando os métodos
aluno.exibirInformacoes(); // Exibe nome e idade

console.log("Média das notas:", aluno.calcularMedia()); // Exibe a média
```

**Explicação do Projeto**:

* **Propriedades**: O objeto `aluno` tem propriedades `nome`, `idade`, e `notas` (um array de notas).
* **Métodos**: `exibirInformacoes` exibe o nome e a idade, enquanto `calcularMedia` calcula a média das notas.

**Atividade Guiada**: Adicione uma nova nota ao array `notas` e testar o cálculo da média novamente.
