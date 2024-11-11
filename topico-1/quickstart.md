---
icon: node
---

# Configuração do Ambiente

### **O que é uma IDE?**

Uma **IDE** (Integrated Development Environment) é um software que reúne várias ferramentas de programação em um único lugar, facilitando o desenvolvimento de código. Em uma IDE, você pode:

* Escrever e editar código com **realce de sintaxe** e **auto-completar**, o que ajuda a identificar erros rapidamente.
* Organizar arquivos e pastas de projeto.
* Executar, depurar e testar o código diretamente.
* Usar **extensões** para adicionar funcionalidades, como integração com o Git, formatação de código, entre outras.

#### Visual Studio Code (VSCode)

O Visual Studio Code é uma IDE flexível e completa, que oferece todas as ferramentas necessárias para programar em JavaScript, desde a escrita e organização do código até a execução e depuração. Para quem está começando, ele é fácil de configurar e possui muitas extensões que ajudam a simplificar o desenvolvimento.

***

## Instalando Node JS

Para rodar JavaScript fora do navegador, usaremos o **Node.js**, uma plataforma que permite executar código JavaScript no terminal. Vamos começar configurando o ambiente:

1. **Instale o Node.js**: Acesse o site oficial [Node.js](https://nodejs.org/) e faça o download e instalação.
2. **Testando a Instalação**: Abra o terminal e digite:

```bash
node -v
```

Isso deve mostrar a versão do Node.js instalada, confirmando que tudo está funcionando.

1. **Executando JavaScript com Node.js**:
   * No terminal, digite `node` e pressione Enter para entrar no console do Node.js.
   * Agora, você pode digitar comandos JavaScript e ver o resultado imediatamente.

Digite o seguinte código no console do Node.js e pressione Enter:

```javascript
console.log("Hello, World!");
```

O Node.js vai exibir `Hello, World!`, mostrando que o ambiente está funcionando corretamente.

***

### **Executando** nosso código

Para facilitar a execução e teste dos códigos, crie um arquivo com a extensão `.js` em seu diretório de projetos, por exemplo, em `logica-de-programacao/index.js`

No arquivo `index.js`, digite o seguinte código para testar:

```javascript
console.log("Olá, mundo! Este é meu primeiro código em Node.js!");
```

**Executando o Arquivo com Node.js**:

Para executar o arquivo, volte ao terminal e navegue até a pasta onde ele foi salvo.

Digite o seguinte comando:

```bash
node index.js
```

O terminal exibirá:

```css
Olá, mundo! Este é meu primeiro código em Node.js!
```

Essa configuração facilita a execução dos códigos, permitindo que você edite e execute arquivos JavaScript de forma prática e rápida.
