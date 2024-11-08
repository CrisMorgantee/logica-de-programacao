---
icon: display-code
---

# Tarefa para Praticar

Expanda o sistema de cadastro de alunos para incluir uma função `buscarAluno` que receba um nome e retorne o objeto do aluno, caso ele exista, ou uma mensagem dizendo que o aluno não foi encontrado.

#### Dica: Use o método `find` para buscar um item específico em um array.

Divirta-se praticando!

#### **Resposta:**

Primeiro, vamos criar um array de objetos representando os alunos, onde cada aluno tem um nome e uma idade. Em seguida, implementaremos a função `buscarAluno`.

```javascript
// Array de objetos representando alunos
let alunos = [
    { nome: "Ana", idade: 17 },
    { nome: "Carlos", idade: 18 },
    { nome: "Beatriz", idade: 19 },
    { nome: "João", idade: 20 }
];

// Função buscarAluno que recebe um nome e busca o aluno no array
function buscarAluno(nome) {
    const aluno = alunos.find(aluno => aluno.nome === nome);

    // Verifica se o aluno foi encontrado
    if (aluno) {
        return aluno;
    } else {
        return "Aluno não encontrado.";
    }
}

// Exemplos de uso da função buscarAluno
console.log(buscarAluno("Carlos")); 
// Saída: { nome: 'Carlos', idade: 18 }

console.log(buscarAluno("Mariana")); 
// Saída: "Aluno não encontrado."
```

#### **Explicação da Função `buscarAluno`**

1. **Parâmetro `nome`**: A função `buscarAluno` recebe um nome como argumento e tenta encontrar um aluno com esse nome no array `alunos`.
2. **Método `find`**: O método `find` percorre o array `alunos` e retorna o primeiro objeto que satisfaz a condição `aluno.nome === nome`.
3. **Verificação de Resultado**:
   * Se o aluno for encontrado, a função retorna o objeto do aluno.
   * Se o aluno não for encontrado, a função retorna a mensagem `"Aluno não encontrado."`.

#### **Exemplos de Saída**

1. **`buscarAluno("Carlos")`**: Como "Carlos" existe no array `alunos`, a função retorna `{ nome: "Carlos", idade: 18 }`.
2. **`buscarAluno("Mariana")`**: Como "Mariana" não existe no array, a função retorna a mensagem `"Aluno não encontrado."`.
