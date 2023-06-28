# Quem Sou Eu?

--

> ### Gabriel Traldi
> Engenheiro de Software Front-End
>
> Time Consultoria

--

## Contato

- Email: gtraldi@viceri.com.br
- LinkedIn: [linkedin.com/in/gabriel-traldi](https://www.linkedin.com/in/gabriel-traldi-235b16133/)
- GitHub: [github.com/Gabriel-Traldi](https://github.com/Gabriel-Traldi)

---
# Guilda Front-End

--

As guildas são grupos de pessoas que compartilham interesses em áreas específicas.

As guildas podem ser formadas por desenvolvedores, engenheiros de softwares, designers, pessoas de áreas não técnicas, como marketing e RH. 

--

O objetivo é promover a colaboração e a troca de conhecimento dentro da empresa.

--

As guildas serão auto-organizadas e possuirão um líder ou facilitador que ajudará a coordenar as atividades do grupo, bem como criar o planejamento, definir calendário, envolver pessoas, etc.

--

A reunião poderá seguir os formatos de:

> Workshops

> Hands On

> Mesa Redonda

--

> [!note] Mesa redonda
> A  mesa redonda pode ser uma reunião, onde, com um facilitador, mais de uma pessoa (as vezes todas), poderão expor a sua opinião (em forma de debate ou não), sobre um determinado assunto. É importante que exista um facilitador, justamente com ideias/perguntas, para fazer com que a reunião flua.

--

> [!note] Workshops
> Um workshop é uma atividade que visa desenvolver habilidades específicas em um ambiente de grupo. O objetivo de um workshop é compartilhar conhecimento, técnicas e melhores práticas, geralmente através de apresentações, discussões e exercícios práticos. Em geral, um workshop é mais focado em teoria e conceitos, com uma abordagem mais didática.

--

> [!note] Hands-on
> O hands-on é uma abordagem mais prática de aprendizado, em que o aprendiz tem a oportunidade de trabalhar diretamente com a tecnologia ou produto em questão. Nesse tipo de atividade, os participantes colocam a mão na massa. O objetivo é fornecer uma experiência mais real.

--

As reuniões das guildas poderão ser virtuais ou presenciais e, pelo menos por enquanto, ocorrerão a cada duas semanas, toda quarta-feira.

--

#### Dúvidas?

---
# Eslint, Prettier e Husky, como criar um padrão de escrita no código

--

## ESLint & Prettier

O ESlint é uma ferramenta para identificar e relatar padrões encontrados no código (ES/JS/TS), analisando o código estaticamente, de forma rápida, com o objetivo de tornar o código mais consistente e evitar bugs.

O significado da palavra "prettier" é "bonito" e o objetivo é padronizar algumas coisas além do que o Eslint faz. (Limitar tamanho das linhas, adicionar espaçamentos com o objetivo de deixar nosso código mais elegante, etc).

--

## Extensão p/ VS Code

![[Pasted image 20230628145938.png]]

Integra o ESLint ao VS Code, procurará pela versão instalada no "workspace", se não, buscará uma global.

Principal vantagem é que podemos configurar o VS Code para sempre que salvarmos um arquivo, ele formatar o arquivo no padrão do ESLint.

--

## Rules de terceiros

```json
// .eslintrc.json
{
  "extends": [
    "next/core-web-vitals",
    "@rocketseat/eslint-config/react"
  ]
}
```

--

## Settings.json

```json
// settings.json
"editor.codeActionsOnSave": {
	"source.fixAll": true
}
```

--

## Plugins para o Prettier

```js
// prettier.config.js
module.exports = {
  plugins: [require('prettier-plugin-tailwindcss')],
}
```

--

## Git Hoooks

Maneira para disparar scripts quando certa ação ocorre. 

Exemplo: `commit`.

--

## Husky

Ferramenta para manusear os git hooks de forma fácil.

---

## Pesquisa

---
## Referências

- [ESLint](https://eslint.org/)
- [Prettier](https://prettier.io/)
- [ESLint VS Code](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint#:~:text=will%20validate%20files%20inside%20the,directory%20to%20the%20provided%20directories.)
- [Git Hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks)
- [husky](https://typicode.github.io/husky/)