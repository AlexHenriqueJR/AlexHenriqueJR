# Projeto Fullstack - React + Node.js

Este é um projeto fullstack desenvolvido com React no frontend e Node.js no backend. O projeto oferece funcionalidades de cadastro e login com autenticação JWT.

## Tecnologias Utilizadas

- **Frontend**: React, React Router, CSS
- **Backend**: Node.js, Express, JWT (JSON Web Token), MySQL, bcrypt, dotenv
- **Banco de Dados**: MySQL
- **Autenticação**: JWT (JSON Web Token)

## Estrutura do Projeto

### Frontend (React)

O frontend é responsável pela interface do usuário, onde temos as seguintes páginas:

- **Login**: Página de login do usuário.
- **Signup**: Página de cadastro de usuário.
- **Home**: Página inicial acessível apenas para usuários autenticados.
- **ProtectedRoute**: Componente que protege rotas privadas e só permite acesso aos usuários autenticados.

### Backend (Node.js)

O backend é responsável pela autenticação dos usuários, com rotas de login e cadastro, além de geração de tokens JWT para garantir a segurança das rotas protegidas.

#### Principais Funcionalidades

- **Cadastro de usuário**: Cria um novo usuário com validação de e-mail e criptografia de senha.
- **Login de usuário**: Permite o login com validação de senha e geração de um token JWT para o usuário.
- **Proteção de rotas**: O token JWT é utilizado para proteger rotas e garantir que apenas usuários autenticados possam acessá-las.

### Rotas do Backend

- **POST /Signup**: Rota para cadastrar um novo usuário.
  - **Parâmetros**:
    - `username`: Nome de usuário.
    - `email`: E-mail do usuário.
    - `password`: Senha do usuário (será criptografada).
  - **Resposta**: Retorna um token JWT se o cadastro for bem-sucedido ou uma mensagem de erro se houver algum problema (ex: e-mail já cadastrado).

- **POST /login**: Rota para realizar o login de um usuário.
  - **Parâmetros**:
    - `email`: E-mail do usuário.
    - `password`: Senha do usuário.
  - **Resposta**: Retorna um token JWT se as credenciais estiverem corretas ou uma mensagem de erro se as credenciais forem inválidas.

### Como Executar o Projeto

Executar Servidor : Dentro da pasta Serve. Executar o comando : npm start serve.js. 

Na pasta Raiz : executar o comando : Npm run dev.

Para efetuar os test : na pasta Serve exetucu o comando : npm run test. 


<!---
AlexHenriqueJR/AlexHenriqueJR is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
