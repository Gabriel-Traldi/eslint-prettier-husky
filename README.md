# Projeto Next.js com Eslint, Prettier, Husky e Lint-Staged

O objetivo deste projeto é demonstrar o funcionamento das ferramentas Eslint, Prettier, Husky e Lint-Staged, que são amplamente utilizadas para padronização de código, formatação automática e verificação de qualidade em projetos JavaScript.

## Sobre o Projeto

Este repositório foi criado com o propósito de apresentar as funcionalidades do Eslint, Prettier, Husky e Lint-Staged e como eles podem ser integrados a um projeto Next.js.

## Funcionalidades

Este projeto utiliza as seguintes ferramentas:

- **Eslint**: O Eslint é uma ferramenta de análise estática que ajuda a identificar e reportar problemas de qualidade de código. Ele pode ser configurado com regras personalizadas para garantir que o código siga um padrão específico.

- **Prettier**: O Prettier é um formatador de código que ajuda a manter uma formatação consistente em todo o projeto. Ele pode ser configurado com regras de formatação personalizadas, como espaçamento, quebras de linha, etc.

- **Husky**: O Husky é uma ferramenta que permite a execução de scripts antes de determinados eventos do Git, como commits e pushes. Isso permite a execução automática de tarefas, como a verificação de qualidade de código, antes de enviar as alterações para o repositório remoto.

- **Lint-Staged**: O Lint-Staged é uma ferramenta que permite a execução de scripts apenas nos arquivos modificados em um determinado commit. Isso é útil para evitar a execução de tarefas demoradas em todo o código do projeto. No caso deste projeto, o Lint-Staged é utilizado para executar o Eslint e o Prettier apenas nos arquivos alterados antes de fazer um commit.

## Configuração e Utilização

Para configurar e utilizar este projeto em sua máquina local, siga as etapas abaixo:

1. Clone este repositório em sua máquina:

   ```bash
   git clone https://github.com/gabriel-traldi/eslint-prettier-husky.git
   ```

2. Navegue até o diretório do projeto:

   ```bash
   cd eslint-prettier-husky
   ```

3. Instale as dependências do projeto:

   ```bash
   npm install
   ```

4. Execute o projeto em modo de desenvolvimento:

   ```bash
   npm run dev
   ```

Durante o desenvolvimento, as ferramentas Eslint, Prettier, Husky e Lint-Staged já estão configuradas para funcionar automaticamente. Ao fazer um commit das alterações, o Husky executará as tarefas de verificação de qualidade de código e formatação automaticamente.
