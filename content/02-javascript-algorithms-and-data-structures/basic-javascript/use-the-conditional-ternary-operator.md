---
id: 587d7b7e367417b2b2512b24
title: Use o Operador Condicional (Ternário)
challengeType: 1
forumTopicId: 301181
dashedName: use-the-conditional-ternary-operator
---

# --description--

O <dfn>operador condicional</dfn>, também chamado de <dfn>operador ternário</dfn>, pode ser usado como uma expressão if-else de uma linha.

A sintaxe é:

`condition ? expression-if-true : expression-if-false;`

A função a seguir usa uma instrução if-else para verificar uma condição:

```js
function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```

Isso pode ser reescrito usando o `operador condicional`:

```js
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater";
}
```

# --instructions--

Use o `operador condicional` na função `checkEqual` para verificar se dois números são iguais ou não. A função deve retornar "Equal" ou "Not Equal".

# --hints--

`checkEqual` deve usar o `operador condicional`

```js
assert(/.+?\s*?\?\s*?.+?\s*?:\s*?.+?/.test(code));
```

`checkEqual(1, 2)` deve retornar "Not Equal"

```js
assert(checkEqual(1, 2) === 'Not Equal');
```

`checkEqual(1, 1)` deve retornar "Equal"

```js
assert(checkEqual(1, 1) === 'Equal');
```

`checkEqual(1, -1)` deve retornar "Not Equal"

```js
assert(checkEqual(1, -1) === 'Not Equal');
```

# --seed--

## --seed-contents--

```js
function checkEqual(a, b) {

}

checkEqual(1, 2);
```

# --solutions--

```js
function checkEqual(a, b) {
  return a === b ? "Equal" : "Not Equal";
}
```
