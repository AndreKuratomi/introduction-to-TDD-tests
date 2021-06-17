# Katas ES6

Neste exercício, você converterá uma série de expressões e funções escritas em es5 para serem usadas com es6.

# Início

Para começar você precisa fazer isso:

1. instalar dependências
1. executar testes
1. completar katas

## Instalando Dependências

Para instalar dependências, faça o *fork [deste repositório](https://gitlab.com/kenzie-academy-brasil/se/fe/code-quality/s_katas-6), e clone-o* para sua máquina. A partir da raiz do repositório. Lembre-se que, porque você está fazendo o *fork* do repositório, não é necessário criar um novo diretório ou executar `npm init` nele primeiro. Quando tiver com o repositório em sua máquina, você pode instalar as dependências a partir da raiz do repositório usando o `npm`:

```bash
npm install
```

## Executando Testes

O resultado dos testes será um sinal do quão perto você estará de completar os diversos katas. Você deve executar o seguinte comando em um novo terminal:

```bash
npm test
```

Então, deve aparecer um resultado como este: 

![test output screenshot](https://raw.githubusercontent.com/kenzieacademy/es6-katas/master/test_output.png)

Aqui você pode ver que temos várias falhas, bem como uma ideia do que estamos esperando.

### Completando Katas

Você encontrará funções e expressões escritas em es5 com comentários acima delas explicando quais features do es6 gostaríamos que você usasse para convertê-las. Por exemplo, o primeiro kata, "arrow functions", diz para você converter a função add para uma função arrow. Portanto, você converteria isso:

```js
function add(x, y) {
   return x + y;
}
```

nisso para passar nos testes:

```js
const add = (x, y) => {
   return x + y;
};
```

Depois de completar esta avaliação, adicione ka-br-correcoes (grupo do GitLab) ao seu repositório como Reporter e envie a URL de seu repositório.

# Dúvidas Frequentes

- *O que são [mocha](https://mochajs.org/) e [chai](http://www.chaijs.com/)?* São bibliotecas que facilitam escrever testes unitários. Se tivéssemos usado apenas `console.assert`, não teríamos tido a habilidade de fornecer dicas tão úteis assim sobre como resolver cada kata.
- *Em `package.json`, eu vi que as bibliotecas de teste são escritas em `devdependencies`, em vez de `dependencies`, por que?* Usamos `dependencies` para bibliotecas que são *obrigatórias* para a execução da aplicação, e `devdependencies` para bibliotecas que auxiliam no desenvolvimento de uma aplicação, mas que não são necessárias para que ela rode de fato. Neste caso em particular, a aplicação é apenas um punhado de katas, e, tecnicamente, nós podemos usar tais funções sem executar testes, portanto `devdependencies` é usado.
