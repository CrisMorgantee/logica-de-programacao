---
icon: address-card
---

# Projeto Integrador: Sistema de Cadastro de Alunos

## **Objetivo do Projeto**

&#x20;Criar um sistema de cadastro de alunos com funcionalidades de adição, remoção, filtragem e cálculo da média das notas. Esse projeto integra o uso de arrays, objetos e funções, além de métodos avançados para manipulação de dados.

### **Passo a Passo**

**Passo 1**: Crie um array vazio chamado `alunos` que armazenará os objetos representando cada aluno.

```javascript
let alunos = [];
```

**Passo 2**: Função `adicionarAluno` que recebe nome, idade e nota e adiciona um novo aluno ao array `alunos`.

```javascript
function adicionarAluno(nome, idade, nota) {
    alunos.push({ nome, idade, nota });
}

adicionarAluno("Ana", 16, 8);
adicionarAluno("Carlos", 17, 6);
```

**Passo 3**: Função `removerAluno` que remove um aluno do array `alunos` pelo nome.

```javascript
function removerAluno(nome) {
    alunos = alunos.filter(aluno => aluno.nome !== nome);
}

removerAluno("Carlos");

console.log(alunos); // Deve mostrar apenas o aluno "Ana"
```

**Passo 4**: Função `filtrarAprovados` que filtra os alunos com nota maior ou igual a 7.

```javascript
function filtrarAprovados() {
    return alunos.filter(aluno => aluno.nota >= 7);
}

console.log(filtrarAprovados()); // Exibe os alunos aprovados
```

**Passo 5**: Função `calcularMedia` que calcula a média das notas de todos os alunos.

```javascript
function calcularMedia() {
    if (alunos.length === 0) return 0;
    let soma = alunos.reduce((total, aluno) => total + aluno.nota, 0);
    return soma / alunos.length;
}

console.log("Média Geral:", calcularMedia());
```

**Código Completo do Projeto**:

```javascript
let alunos = [];

function adicionarAluno(nome, idade, nota) {
    alunos.push({ nome, idade, nota });
}

function removerAluno(nome) {
    alunos = alunos.filter(aluno => aluno.nome !== nome);
}

function filtrarAprovados() {
    return alunos.filter(aluno => aluno.nota >= 7);
}

function calcularMedia() {
    if (alunos.length === 0) return 0;
    let soma = alunos.reduce((total, aluno) => total + aluno.nota, 0);
    return soma / alunos.length;
}

// Testando o sistema
adicionarAluno("Ana", 16, 8);
adicionarAluno("Carlos", 17, 6);

console.log("Alunos:", alunos);
console.log("Aprovados:", filtrarAprovados());
console.log("Média Geral:", calcularMedia());

removerAluno("Carlos");

console.log("Alunos após remoção:", alunos);
```

**Explicação do Projeto**:

* **Adicionar Aluno**: `adicionarAluno` permite inserir novos alunos no sistema.
* **Remover Aluno**: `removerAluno` remove um aluno pelo nome, usando `filter` para criar um novo array sem o aluno removido.
* **Filtrar Aprovados**: `filtrarAprovados` retorna um array com alunos cuja nota é maior ou igual a 7.
* **Calcular Média**: `calcularMedia` calcula a média de notas de todos os alunos usando `reduce`.

**Atividade Guiada**: Peça para os alunos testarem o sistema adicionando e removendo alunos e verificando a média geral das notas.
