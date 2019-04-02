# Node - Desafio 4

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/node-desafio4/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/node-desafio4.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/node-desafio4.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/node-desafio4.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/node-desafio4.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/node-desafio4.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/node-desafio4.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

xAplicação usando Node.js, AdonisJs, ESLint, Moment, Raven-node, Mailtrap e Sentry.

## Desafio 4

No desafio final você criará uma API REST com AdonisJS para um sistema de agendamentos de compromissos (calendário). Deixe toda estrutura com ESLint, EditorConfig, etc, que configuramos até agora pronta.

### Requisitos funcionais

- O usuário deve poder criar uma conta com nome, e-mail e senha;
- O usuário deve poder se autenticar na aplicação com e-mail e senha;
- O usuário deve poder alterar seu nome e senha informando a senha antiga, a senha nova e a confirmação da senha nova;
- O usuário deve poder cadastrar eventos em seu calendário com título, localização, data e horário;
- O usuário deve poder listar os eventos cadastrados por data;
- O usuário deve poder excluir um compromisso;
- O usuário deve poder compartilhar um compromisso informando o e-mail do destinatário. Assim que compartilhado, o destinatário deve receber todas informações do evento por e-mail;

### Requisitos não funcionais

- Utilize banco de dados SQL;
- Utilize fila com Redis para programar o envio de e-mails do compartilhamento de compromisso;

### Regras de negócio

- O e-mail do usuário é único;
- O usuário não pode alterar seu e-mail;
- Não deve ser possível cadastrar dois eventos no mesmo horário no calendário de um usuário;
- O usuário só pode ver/editar/deletar seus eventos;
- O usuário não pode editar/deletar um evento que já passou;
- Todos cadastros devem possuir validação de campos com mensagens legíveis;

## Índice

- [Rotas](#rotas)

- [Desenvolvimento](#desenvolvimento)

  - [Configurações Iniciais](#configurações-iniciais)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Execução do Projeto](#execução-do-projeto)

  - [Execução de API para Desenvolvimento](#execução-de-api-para-desenvolvimento)

  - [Execução de Ouvinte de Fila](#execução-de-ouvinte-de-fila)

  - [Bibliotecas](#bibliotecas)

  - [Outras Ferramentas](#outras-ferramentas)

## Rotas

x- Projetos

  - Lista todos os projetos
  - Adiciona novos projetos
  - Lista somente dados de um projeto
  - Edita dados de projetos existentes
  - Exclui projetos existentes

x- Tarefas

  - Lista todas as tarefas de um projeto
  - Adiciona novas tarefas em um projeto
  - Lista somente dados de uma tarefa de um projeto
  - Edita dados de uma tarefa de um projeto
  - Exclui uma tarefa de um projeto

x- Arquivos

  - Lista um arquivo
  - Adiciona novos arquivos

x- Redefinição de Senha

  - Requisita nova senha
  - Adiciona nova senha

x- Sessões

  - Adiciona novas sessões

x- Usuários

  - Adiciona novos usuários

## Desenvolvimento

### Configurações Iniciais

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga as Configurações Iniciais.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga a Instalação de Projeto.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga a Execução de Projeto.

### Execução de API para Desenvolvimento

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-cli.md) e siga a Execução de API para Desenvolvimento.

### Execução de Ouvinte de Fila

xClique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-cli.md) e siga a Execução de Ouvinte de Fila.

### Bibliotecas

x- [Adonis Kue Provider](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/adonis-kue.md)

x- [Adonis Mail](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-mail.md)

x- [Adonis Validator](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-validator.md)

- [AdonisJs Cli](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-cli.md)

x- [AdonisJs Redis](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@adonisjs-redis.md)

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

x- [Moment](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/moment.md)

- [pg](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/pg.md)

x- [Raven-node](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/raven.md)

### Outras Ferramentas

- [DBeaver](https://github.com/osvaldokalvaitir/projects-settings/blob/master/database/dbeaver.md)

- [Docker](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/docker.md)

  - Imagem do PostgreSQL: [kartoza-postgis](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/kartoza-postgis.md)

  - Imagem do Redis: [redis:alpine](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/redis-alpine.md)

- [Mailtrap](https://github.com/osvaldokalvaitir/projects-settings/blob/master/email/mailtrap.md)

- [Insomnia](https://github.com/osvaldokalvaitir/projects-settings/blob/master/api/insomnia.md)

- [Sentry](https://github.com/osvaldokalvaitir/projects-settings/blob/master/error/sentry.md)
