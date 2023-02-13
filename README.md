# NodeJS Fundamentals - Challenge 🔥

<p align="center">
  <img src="https://img.shields.io/static/v1?label=challenge&message=nodejs-fundamentals&color=blueviolet&style=for-the-badge"/>
  <img src="https://img.shields.io/github/license/MrRioja/nodejs-fundamentals-challenge?color=blueviolet&logo=License&style=for-the-badge"/>
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/MrRioja/nodejs-fundamentals-challenge?color=blueviolet&logo=JavaScript&logoColor=white&style=for-the-badge">
  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/MrRioja/nodejs-fundamentals-challenge?color=blueviolet&style=for-the-badge">
</p>

<p align="center">
  <a href="#sobre">Sobre</a> •
  <a href="#fundamentos-do-nodejs---challenge">Fundamentos do NodeJS - Challenge</a> •
  <a href="#instalação">Instalação</a> •
  <a href="#tecnologias">Tecnologias</a> •
  <a href="#autor">Autor</a>  
</p>

## Sobre

Desafio proposto no primeiro módulo do Bootcamp Ignite 2023 na trilha de NodeJS.

## Fundamentos do NodeJS - Challenge

Desafio proposto na trilha de NodeJS do bootcamp Ignite 2023 no módulo: **Fundamentos do NodeJS**.

O desafio proposto foi criar uma API para realizar o CRUD de tarefas. A aplicação contem as seguintes funcionalidades:

- [x] Criação de task.
- [x] Listagem de todas as tasks.
- [x] Atualização de uma task pelo `id`.
- [x] Remoção uma task pelo `id`.
- [x] Marcar pelo `id` uma task como completa.
- [x] Importação de tasks em massa por um arquivo CSV.

As tasks possuem as seguintes propriedades:

- **_id_** - Identificador único de cada task.
- **_title_** - Título da task.
- **_description_** - Descrição detalhada da task.
- **_completed_at_** - Data de quando a task foi concluída. O valor inicial deve ser `null`.
- **_created_at_** - Data de quando a task foi criada.
- **_updated_at_** - Deve ser sempre alterado para a data de quando a task foi atualizada.

### Rotas da aplicação

<details>
  <summary>GET - <code>/tasks</code></summary>
  <br>
    Lista todas as tasks salvas no banco de dados. Também é possível realizar uma busca, filtrando as tasks pelo <code>title</code> e <code>description</code>.
</details>

<details>
  <summary>POST - <code>/tasks</code></summary>
  <br>
  Cria uma task no banco de dados com os campos <code>title</code> e <code>description</code> recebidos por meio do <code>body</code> da requisição.
  Ao criar uma task, os campos: <code>id</code>, <code>created_at</code>, <code>updated_at</code> e <code>completed_at</code> são preenchidos automaticamente, conforme a descrição das propriedades de uma task acima.
</details>

<details>
  <summary>PUT - <code>/tasks/:id</code></summary>
  <br>
  Rota para atualizar uma task pelo <code>id</code>.
  O <code>body</code> da requisição, deve conter somente o <code>title</code> e/ou <code>description</code> para serem atualizados. Se for enviado somente o <code>title</code>, significa que o <code>description</code> não será atualizado e vice-versa.
</details>

<details>
  <summary>DELETE - <code>/tasks/:id</code></summary>
  <br>
  Remove uma task pelo <code>id</code>.
</details>

<details>
  <summary>PATCH - <code>/tasks/:id/complete</code></summary>
  <br>
  Marca uma task como completa ou incompleta.
</details>

As rotas para testar a API da solução do desafio estão disponíveis no botão abaixo:

[![Run in Insomnia}](https://insomnia.rest/images/run.svg)](https://insomnia.rest/run/?label=nodejs-fundamentals-challenge&uri=https://github.com/MrRioja/nodejs-fundamentals-challenge/blob/b4019ef59c0b67c9a0df94be5ae336c346a4acab/.github/Insomnia_2023-02-12.json)

## Instalação

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com) e [Node.js](https://nodejs.org/en/). Além disso é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/).

### 🎲 Rodando o Back End (servidor)

```bash
# Clone este repositório
$ git clone git@github.com:MrRioja/nodejs-fundamentals-challenge.git

# Acesse a pasta do projeto no terminal/cmd
$ cd nodejs-fundamentals-challenge

# Instale as dependências
$ npm install
# Caso prefira usar o Yarn execute o comando abaixo
$ yarn

# Execute a aplicação em modo de desenvolvimento
$ npm run dev
# Caso prefira usar o Yarn execute o comando abaixo
$ yarn dev

# Para executar a criação das tasks por CSV execute
$ npm run import:csv
# Caso prefira usar o Yarn execute o comando abaixo
$ yarn import:csv

# O servidor iniciará na porta 3333 - acesse <http://localhost:3333>
```

## Tecnologias

[![My Skills](https://skillicons.dev/icons?i=nodejs,js)](https://skillicons.dev)

## Autor

<div align="center">
<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/55336456?v=4&h=100&w=100&fit=cover&mask=circle&maxage=7d" />
<h1>Luiz Rioja</h1>
<strong>Backend Developer</strong>
<br/>
<br/>

<a href="https://linkedin.com/in/luizrioja" target="_blank">
<img alt="LinkedIn" src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="https://github.com/mrrioja" target="_blank">
<img alt="GitHub" src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<a href="mailto:lulyrioja@gmail.com?subject=Fala%20Dev" target="_blank">
<img alt="Gmail" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

<a href="https://api.whatsapp.com/send?phone=5511933572652" target="_blank">
<img alt="WhatsApp" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>
</a>

<a href="https://join.skype.com/invite/tvBbOq03j5Uu" target="_blank">
<img alt="Skype" src="https://img.shields.io/badge/SKYPE-%2300AFF0.svg?style=for-the-badge&logo=Skype&logoColor=white"/>
</a>

<br/>
<br/>
</div>
