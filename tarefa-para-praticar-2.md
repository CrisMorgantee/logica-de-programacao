---
icon: display-code
---

# Tarefa para Praticar

Crie um array de objetos representando uma lista de filmes, onde cada filme tem título, diretor e duração (em minutos). Em seguida, use os métodos `map`, `filter` e `reduce` para manipular a lista de filmes.

#### Dicas:

* `map`: Crie uma lista de títulos dos filmes.
* `filter`: Filtre filmes por um diretor específico.
* `reduce`: Calcule a duração total dos filmes.

Divirta-se praticando!

#### **Resposta:**

**Passo 1: Criar o Array de Objetos**

```javascript
// Array de filmes, onde cada filme tem título, diretor e duração em minutos
let filmes = [
    { titulo: "A Origem", diretor: "Christopher Nolan", duracao: 148 },
    { titulo: "Interstellar", diretor: "Christopher Nolan", duracao: 169 },
    { titulo: "Dunkirk", diretor: "Christopher Nolan", duracao: 106 },
    { titulo: "Parasita", diretor: "Bong Joon-ho", duracao: 132 },
    { titulo: "O Hospedeiro", diretor: "Bong Joon-ho", duracao: 119 },
    { titulo: "Whiplash", diretor: "Damien Chazelle", duracao: 107 }
];
```

**Passo 2: Utilizar os Métodos `map`, `filter` e `reduce`**

**`map`** - Criar uma lista com os títulos dos filmes:

```javascript
let titulos = filmes.map(filme => filme.titulo);

console.log("Títulos dos Filmes:", titulos);
// Saída: ["A Origem", "Interstellar", "Dunkirk", "Parasita", "O Hospedeiro", "Whiplash"]
```

**`filter`** - Filtrar filmes dirigidos por "Christopher Nolan":

```javascript
let filmesDoNolan = filmes.filter(filme => filme.diretor === "Christopher Nolan");

console.log("Filmes do Diretor Christopher Nolan:", filmesDoNolan);
/* Saída:
[
    { titulo: "A Origem", diretor: "Christopher Nolan", duracao: 148 },
    { titulo: "Interstellar", diretor: "Christopher Nolan", duracao: 169 },
    { titulo: "Dunkirk", diretor: "Christopher Nolan", duracao: 106 }
]
*/
```

**`reduce`** - Calcular a duração total de todos os filmes:

```javascript
let duracaoTotal = filmes.reduce((acumulador, filme) => acumulador + filme.duracao, 0);

console.log("Duração Total dos Filmes:", duracaoTotal);
// Saída: 781 minutos
```

#### **Explicação dos Métodos Utilizados**

**`map`**:

* `filmes.map(filme => filme.titulo)` cria um novo array contendo apenas os títulos dos filmes.
* **Resultado**: `["A Origem", "Interstellar", "Dunkirk", "Parasita", "O Hospedeiro", "Whiplash"]`

**`filter`**:

* `filmes.filter(filme => filme.diretor === "Christopher Nolan")` cria um novo array contendo apenas os filmes dirigidos por "Christopher Nolan".
* **Resultado**: Lista de objetos com os filmes do diretor especificado.

**`reduce`**:

* `filmes.reduce((acumulador, filme) => acumulador + filme.duracao, 0)` calcula a soma de todas as durações dos filmes no array `filmes`. O `0` no final é o valor inicial do acumulador.
* **Resultado**: `781 minutos`
