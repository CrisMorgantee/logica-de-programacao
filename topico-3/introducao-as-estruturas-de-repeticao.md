---
icon: repeat
---

# Introdução às Estruturas de Repetição

## **O que são Estruturas de Repetição?**

Estruturas de repetição permitem que o computador execute uma mesma ação várias vezes sem precisar escrever o mesmo código repetidamente. Isso é útil quando queremos, por exemplo, contar números, percorrer listas ou executar tarefas repetitivas.

* &#x20;Imagine que você tem que contar de 1 a 10. Você poderia escrever cada número separadamente, ou pedir ao computador para fazer isso por você usando uma estrutura de repetição.

#### **Tipos de Estruturas de Repetição**

1. **`for`**: Usado quando sabemos quantas vezes queremos repetir uma tarefa.
2. **`while`**: Usado quando queremos repetir a tarefa enquanto uma condição for verdadeira.
3. **`do while`**: Similar ao `while`, mas garante que o código será executado ao menos uma vez.

***

### **Estrutura `for`**&#x20;

#### **Como Funciona o `for`?**

O `for` é ideal quando sabemos o número exato de repetições que precisamos. Ele tem três partes:

* **Inicialização**: Define o ponto de partida.
* **Condição**: Verifica se a repetição deve continuar.
* **Incremento**: Atualiza a variável de controle.

**Exemplo Prático**:

```javascript
for (let i = 1; i <= 5; i++) {
    console.log("Contagem:", i);
}
```

**Explicação do Exemplo**:

* **Inicialização**: `let i = 1` define que a contagem começa em 1.
* **Condição**: `i <= 5` significa que o laço vai parar quando `i` for maior que 5.
* **Incremento**: `i++` aumenta `i` em 1 a cada repetição.

Esse código vai exibir:

```makefile
Contagem: 1
Contagem: 2
Contagem: 3
Contagem: 4
Contagem: 5
```

**Atividade Guiada**: Altere o valor inicial, a condição ou o incremento, e observe como isso muda o resultado.

***

### **Estrutura `while`**&#x20;

#### **Como Funciona o `while`?**

O `while` repete uma tarefa enquanto uma condição for verdadeira. É útil quando não sabemos o número exato de repetições, mas temos uma condição a ser atendida.

**Exemplo Prático**:

```javascript
let contador = 1;

while (contador <= 3) {
    console.log("Número:", contador);
    contador++;
}
```

**Explicação do Exemplo**:

* **Inicialização**: `let contador = 1` define o ponto de partida.
* **Condição**: `contador <= 3` mantém o loop ativo enquanto `contador` for menor ou igual a 3.
* **Incremento**: `contador++` aumenta `contador` em 1 a cada repetição.

Esse código vai exibir:

```makefile
Número: 1
Número: 2
Número: 3
```

**Atividade Guiada**: Altere a condição do loop para ver o que acontece quando a condição não é atendida.

***

### **Estrutura `do while`**&#x20;

#### **Como Funciona o `do while`?**

O `do while` é semelhante ao `while`, mas garante que o bloco de código seja executado ao menos uma vez, mesmo se a condição for falsa desde o início.

**Exemplo Prático**:

```javascript
let numero = 6;

do {
    console.log("Número atual:", numero);
    numero++;
} while (numero <= 5);
```

**Explicação do Exemplo**:

* Esse código executa `console.log("Número atual:", numero);` uma vez, mesmo que `numero` seja maior que 5 desde o início. Isso acontece porque a condição é verificada após a primeira execução do bloco.

Esse código vai exibir:

```mathematica
Número atual: 6
```

O `do while` é menos comum, mas pode ser útil em situações específicas onde precisamos de uma execução garantida.
