---
icon: books
---

# Projeto Prático: Biblioteca de Livros

## **Objetivo do Projeto**&#x20;

Criar um sistema básico de gerenciamento de biblioteca usando arrays e objetos. A biblioteca será um array de objetos, onde cada objeto representa um livro com título, autor e número de páginas.

### **Passo a Passo**

**Passo 1**: Crie o array `biblioteca` com alguns objetos representando livros.

```javascript
let biblioteca = [
    { titulo: "Livro A", autor: "Autor 1", paginas: 200 },
    { titulo: "Livro B", autor: "Autor 2", paginas: 150 },
    { titulo: "Livro C", autor: "Autor 1", paginas: 300 }
];
```

**Passo 2**: Use `map` para criar uma lista de títulos dos livros.

```javascript
let titulos = biblioteca.map(livro => livro.titulo);

console.log(titulos); // ["Livro A", "Livro B", "Livro C"]
```

**Passo 3**: Use `filter` para encontrar todos os livros de um autor específico.

```javascript
let livrosDoAutor1 = biblioteca.filter(livro => livro.autor === "Autor 1");

console.log(livrosDoAutor1);
```

**Passo 4**: Use `reduce` para calcular o total de páginas da biblioteca.

```javascript
let totalPaginas = biblioteca.reduce((total, livro) => total + livro.paginas, 0);

console.log("Total de páginas:", totalPaginas); // Exemplo de saída: Total de páginas: 650
```

**Código Completo**:

```javascript
let biblioteca = [
    { titulo: "Livro A", autor: "Autor 1", paginas: 200 },
    { titulo: "Livro B", autor: "Autor 2", paginas: 150 },
    { titulo: "Livro C", autor: "Autor 1", paginas: 300 }
];

let titulos = biblioteca.map(livro => livro.titulo);
console.log("Títulos:", titulos);

let livrosDoAutor1 = biblioteca.filter(livro => livro.autor === "Autor 1");
console.log("Livros do Autor 1:", livrosDoAutor1);

let totalPaginas = biblioteca.reduce((total, livro) => total + livro.paginas, 0);
console.log("Total de páginas:", totalPaginas);
```

**Explicação do Projeto**:

* **Mapeamento de Títulos**: `map` permite criar uma lista de títulos dos livros.
* **Filtragem por Autor**: `filter` cria uma lista de todos os livros de um autor específico.
* **Soma de Páginas**: `reduce` permite calcular o número total de páginas da biblioteca.

**Atividade Guiada**: Peça para os alunos adicionarem mais livros ao array `biblioteca` e repetirem os passos de mapeamento, filtragem e redução com os novos dados.

**Discussão e Perguntas (20 minutos)**

* **Objetivo**: Esclarecer dúvidas sobre os métodos `map`, `filter`, `reduce` e os métodos de strings.
* **Discussão**: Pergunte aos alunos como esses métodos facilitam a manipulação de dados e como eles podem ser usados em outras situações.

**Exemplos para Explorar**:

**Pergunte:** "Como vocês poderiam usar esses métodos para organizar dados de uma lista de contatos?"

**Resposta**:

&#x20;Imagine que você tem uma lista de contatos onde cada contato é representado por um objeto com propriedades como `nome`, `telefone`, `email`, e `cidade`. Podemos usar `map`, `filter`, e `reduce` para organizar e manipular esses dados de diferentes formas:

**`map`**: Se quisermos criar uma lista apenas com os nomes dos contatos, podemos usar `map` para extrair o campo `nome` de cada contato. O resultado seria um novo array contendo apenas os nomes.

**Exemplo**:

```javascript
let contatos = [
    { nome: "Ana", telefone: "1234-5678", email: "ana@example.com", cidade: "São Paulo" },
    { nome: "João", telefone: "8765-4321", email: "joao@example.com", cidade: "Rio de Janeiro" },
];

let nomes = contatos.map(contato => contato.nome);

console.log(nomes); // Saída: ["Ana", "João"]
```

**`filter`**: Podemos usar `filter` para encontrar todos os contatos que estão em uma cidade específica, como "São Paulo". Isso criaria uma nova lista contendo apenas os contatos dessa cidade.

**Exemplo**:

```javascript
let contatosDeSaoPaulo = contatos.filter(contato => contato.cidade === "São Paulo");

console.log(contatosDeSaoPaulo);
// Saída: [{ nome: "Ana", telefone: "1234-5678", email: "ana@example.com", cidade: "São Paulo" }]
```

**`reduce`**: Podemos usar `reduce` para contar quantos contatos temos no total ou para agrupar os contatos por cidade, criando um objeto onde as chaves são os nomes das cidades e os valores são arrays de contatos daquela cidade.

**Exemplo de agrupamento por cidade**:

```javascript
let contatosPorCidade = contatos.reduce((acumulador, contato) => {
    if (!acumulador[contato.cidade]) {
        acumulador[contato.cidade] = [];
    }
    acumulador[contato.cidade].push(contato);
    return acumulador;
}, {});

console.log(contatosPorCidade);
/* Saída:
{
    "São Paulo": [{ nome: "Ana", telefone: "1234-5678", email: "ana@example.com", cidade: "São Paulo" }],
    "Rio de Janeiro": [{ nome: "João", telefone: "8765-4321", email: "joao@example.com", cidade: "Rio de Janeiro" }]
}
*/
```

Esses métodos permitem organizar, filtrar e transformar uma lista de contatos de forma muito eficiente.

**Pergunte:** "Qual seria uma situação em que `reduce` seria mais eficiente que um `for`?"

**Resposta**: `reduce` é especialmente eficiente e útil quando queremos combinar ou resumir dados de um array em um único valor ou estrutura (como somar números, contar itens, ou criar agrupamentos). Aqui estão algumas situações em que `reduce` é mais eficiente do que um `for` tradicional:

1.  **Soma ou Contagem de Elementos**:

    Se quisermos somar todos os números de um array, `reduce` permite fazer isso de forma compacta e clara, sem precisar de variáveis adicionais para armazenar o total. Isso simplifica o código, tornando-o mais legível e menos propenso a erros.



    **Exemplo**:

    ```javascript
    let numeros = [1, 2, 3, 4, 5];
    let soma = numeros.reduce((total, num) => total + num, 0);

    console.log(soma); // Saída: 15
    ```
2.  **Agrupamento de Elementos**:

    Para agrupar elementos de um array por uma categoria (como agrupar pessoas por cidade ou produtos por categoria), `reduce` permite criar uma estrutura de dados complexa sem a necessidade de múltiplas variáveis ou loops aninhados. É uma maneira muito mais eficiente e direta de realizar agrupamentos do que `for`.



    **Exemplo**:

    ```javascript
    let produtos = [
        { nome: "Produto A", categoria: "Eletrônicos" },
        { nome: "Produto B", categoria: "Alimentos" },
        { nome: "Produto C", categoria: "Eletrônicos" }
    ];

    let produtosPorCategoria = produtos.reduce((acumulador, produto) => {
        if (!acumulador[produto.categoria]) {
            acumulador[produto.categoria] = [];
        }
        acumulador[produto.categoria].push(produto);
        return acumulador;
    }, {});

    console.log(produtosPorCategoria);
    /* Saída:
    {
        "Eletrônicos": [{ nome: "Produto A", categoria: "Eletrônicos" }, { nome: "Produto C", categoria: "Eletrônicos" }],
        "Alimentos": [{ nome: "Produto B", categoria: "Alimentos" }]
    }
    */
    ```
3.  **Construção de Objetos Complexos**:

    Quando precisamos transformar um array em um objeto com uma estrutura complexa (por exemplo, criar um índice onde cada chave é um item único e o valor é a contagem de vezes que o item aparece), `reduce` é mais eficiente e flexível do que `for`.



    **Exemplo**: Criar um contador de elementos.

    ```javascript
    let palavras = ["maçã", "banana", "maçã", "laranja", "banana", "maçã"];

    let contador = palavras.reduce((acumulador, palavra) => {
        if (!acumulador[palavra]) {
            acumulador[palavra] = 0;
        }
        acumulador[palavra]++;
        return acumulador;
    }, {});

    console.log(contador);
    /* Saída:
    {
        "maçã": 3,
        "banana": 2,
        "laranja": 1
    }
    */
    ```

Essas são situações onde `reduce` se destaca por sua capacidade de transformar e resumir dados de maneira eficiente. O uso do `reduce` permite que o código fique mais enxuto e expressivo, reduzindo a necessidade de variáveis auxiliares e tornando o propósito do código mais claro.
