# 💻 Blog Pessoal API

![Badge da Tecnologia](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Badge da Tecnologia](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Badge da Tecnologia](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Badge da Licença](https://img.shields.io/badge/License-MIT-green.svg)

## 📝 Descrição do Projeto

O **Blog Pessoal API** é uma aplicação backend robusta e escalável desenvolvida utilizando o framework **NestJS**. Ele serve como o núcleo de um sistema de blog, fornecendo a infraestrutura de dados e lógica de negócio (CRUD) para gerenciar postagens e seus respectivos temas ou categorias. O projeto segue a arquitetura modular do NestJS, promovendo alta coesão e baixo acoplamento entre os componentes.

## ✨ Funcionalidades Principais

O sistema é dividido nos seguintes módulos principais: **Módulo Tema (Tema)**, que inclui a Entidade Tema, o Tema Controller (para CRUD de temas) e o Tema Service (para regras de negócio); e o **Módulo Postagem (Postagem)**, que inclui a Entidade Postagem e o Relacionamento 1:N, onde uma Postagem está associada a um Tema e um Tema pode ter múltiplas Postagens. O Postagem Service gerencia a lógica de negócio das postagens, garantindo a integridade do relacionamento.

## 🛠️ Tecnologias Utilizadas

As tecnologias principais são: o framework **NestJS**, a linguagem **TypeScript**, o runtime **Node.js** e o **TypeORM** (assumido como ORM), podendo utilizar bancos de dados como PostgreSQL, MySQL ou SQLite, dependendo da configuração.

## 🚀 Como Executar o Projeto

Para executar localmente, certifique-se de ter **Node.js**, **NPM ou Yarn** e **Git** instalados. Primeiro, clone o repositório (`git clone https://github.com/MariPires96/blog_pessoal.git` e `cd blog_pessoal`), em seguida, instale as dependências (`npm install` ou `yarn install`). Crie um arquivo `.env` para configurar o Banco de Dados. Para rodar em desenvolvimento com *hot reload*, utilize `npm run start:dev` ou `yarn start:dev` (A API estará em `http://localhost:4000`). Para produção, use `npm run build` seguido de `npm run start`.

## 🔗 Endpoints Principais (Exemplos)

Os endpoints incluem, para o **Tema**, `GET /temas` (Listar todos) e `POST /temas` (Cadastrar novo); e para **Postagem**, `GET /postagens` (Listar todas) e `POST /postagens` (Cadastrar nova, requer ID do Tema).
