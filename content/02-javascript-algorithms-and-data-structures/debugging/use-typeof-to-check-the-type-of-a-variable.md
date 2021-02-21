---
id: 587d7b84367417b2b2512b34
title: Use typeof para verificar o tipo de uma variável
challengeType: 1
forumTopicId: 18374
dashedName: use-typeof-to-check-the-type-of-a-variable
---

# --description--

Você pode usar `typeof` para verificar a estrutura de dados, ou tipo, de uma variável. Isso é útil na depuração ao trabalhar com vários tipos de dados. Se você pensa que está adicionando dois números, mas um é na verdade uma string, os resultados podem ser inesperados. Erros de tipo podem se esconder em cálculos ou chamadas de função. Tenha cuidado, especialmente ao acessar e trabalhar com dados externos na forma de um objeto JavaScript Object Notation (JSON).

Aqui estão alguns exemplos usando `typeof`:

```js
console.log(typeof ""); // outputs "string"
console.log(typeof 0); // outputs "number"
console.log(typeof []); // outputs "object"
console.log(typeof {}); // outputs "object"
```

JavaScript reconhece seis tipos de dados primitivos (imutáveis): `Boolean`, `Null`, `Undefined`, `Number`, `String` e `Symbol` (novo no ES6) e um tipo para itens mutáveis: `Object`. Observe que, em JavaScript, os arrays são tecnicamente um tipo de objeto.

# --instructions--

Adicione duas instruções `console.log()` para verificar o `typeof` de cada uma das duas variáveis `seven` e `three` no código.

# --hints--

Seu código deve usar `typeof` em duas instruções `console.log() `para verificar o tipo das variáveis.

```js
assert(code.match(/console\.log\(typeof[\( ].*\)?\)/g).length == 2);
```

Seu código deve usar `typeof` para verificar o tipo da variável `seven`.

```js
assert(code.match(/typeof[\( ]seven\)?/g));
```

Seu código deve usar `typeof` para verificar o tipo da variável `three`.

```js
assert(code.match(/typeof[\( ]three\)?/g));
```

# --seed--

## --seed-contents--

```js
let seven = 7;
let three = "3";
console.log(seven + three);
// Only change code below this line
```

# --solutions--

```js
let seven = 7;let three = "3";console.log(typeof seven);
console.log(typeof three);
```
