---
icon: reel
---

# Manipulação de Strings em JavaScript

## **Métodos de String**

**`toUpperCase` e `toLowerCase`**: Transformam o texto para letras maiúsculas ou minúsculas.

```javascript
let texto = "JavaScript";

console.log(texto.toUpperCase()); // "JAVASCRIPT"
console.log(texto.toLowerCase()); // "javascript"
```

**`slice`**: Extrai uma parte da string e retorna como uma nova string.

```javascript
let frase = "Bem-vindo ao curso de JavaScript";

console.log(frase.slice(0, 9)); // "Bem-vindo"
```

**`includes`**: Verifica se uma substring está contida na string principal.

```javascript
let frase = "Aprendendo JavaScript!";

console.log(frase.includes("JavaScript")); // true
```

**Atividade Guiada**: Crie uma string de exemplo, use `toUpperCase`, `slice`, e `includes` e observe os resultados.
