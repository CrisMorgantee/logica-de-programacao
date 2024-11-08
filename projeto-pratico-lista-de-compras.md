---
icon: list
---

# Projeto Prático: Lista de Compras

## **Objetivo do Projeto**

Criar uma lista de compras usando um array para armazenar os itens. Os alunos poderão adicionar, remover e exibir todos os itens da lista.

### Passo a passo

**Passo 1**: Crie um array vazio chamado `listaDeCompras`.

```javascript
let listaDeCompras = [];
```

**Passo 2**: Adicione alguns itens à lista usando o método `push`.

```javascript
listaDeCompras.push("Leite");
listaDeCompras.push("Pão");
listaDeCompras.push("Queijo");

console.log("Lista de Compras:", listaDeCompras);
```

**Passo 3**: Remova o último item da lista (simulando que você comprou o item).

```javascript
listaDeCompras.pop();

console.log("Lista de Compras (após remover o último item):", listaDeCompras);
```

**Passo 4**: Exiba todos os itens da lista usando um loop `for`.

```javascript
console.log("Itens na Lista de Compras:");

for (let i = 0; i < listaDeCompras.length; i++) {
    console.log(listaDeCompras[i]);
}
```

**Código Completo**:

```javascript
let listaDeCompras = [];

// Adicionar itens à lista
listaDeCompras.push("Leite");
listaDeCompras.push("Pão");
listaDeCompras.push("Queijo");

console.log("Lista de Compras:", listaDeCompras);

// Remover o último item
listaDeCompras.pop();
console.log("Lista de Compras (após remover o último item):", listaDeCompras);

// Exibir todos os itens
console.log("Itens na Lista de Compras:");

for (let i = 0; i < listaDeCompras.length; i++) {
    console.log(listaDeCompras[i]);
}
```

**Explicação do Projeto**:

* **Adição de Itens**: Usamos `push` para adicionar itens à lista.
* **Remoção de Itens**: Usamos `pop` para remover o último item.
* **Exibição de Itens**: Usamos um loop `for` para mostrar cada item na lista.

**Atividade Guiada**: Adicione mais itens à lista, tente remover itens do início usando `shift`.
