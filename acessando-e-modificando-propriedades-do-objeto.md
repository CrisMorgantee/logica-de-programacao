---
icon: bracket-curly
---

# Acessando e Modificando Propriedades do Objeto

## **Acessando Propriedades**

Podemos acessar uma propriedade de um objeto usando a notação de ponto (`.`) ou a notação de colchetes (`[]`).

**Exemplo Prático**:

```javascript
console.log(pessoa.nome); // Saída: Carlos
console.log(pessoa["idade"]); // Saída: 25
```

### **Modificando Propriedades**

Para alterar o valor de uma propriedade, acessamos a propriedade e atribuímos um novo valor.

**Exemplo Prático**:

```javascript
pessoa.idade = 26; // Atualiza a idade para 26

console.log(pessoa.idade); // Saída: 26
```

**Atividade Guiada**: Crie um objeto chamado `carro` com propriedades `marca`, `modelo`, e `ano`, e exibia as propriedades no console.

### **Adicionando Propriedades**

Podemos adicionar uma nova propriedade a um objeto mesmo depois de ele ter sido criado, simplesmente definindo uma nova chave.

**Exemplo Prático**:

```javascript
pessoa.peso = 70; // Adiciona uma nova propriedade "peso"
console.log(pessoa); // Saída: {nome: "Carlos", idade: 26, altura: 1.75, peso: 70}
```

### **Removendo Propriedades**

Podemos remover uma propriedade de um objeto usando o operador `delete`.

**Exemplo Prático**:

```javascript
delete pessoa.altura; // Remove a propriedade "altura"
console.log(pessoa); // Saída: {nome: "Carlos", idade: 26, peso: 70}
```

**Atividade Guiada**: Adicione uma nova propriedade `cor` ao objeto `carro` e depois remova.
