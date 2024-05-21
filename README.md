# Todo App

## Descrição

O Todo App é uma aplicação de lista de tarefas que permite aos usuários gerenciar suas tarefas diárias. A aplicação permite adicionar, visualizar, atualizar e excluir tarefas. O projeto é dividido em duas partes: o backend, que fornece a API RESTful, e o frontend, que fornece a interface de usuário.

## Tecnologias Utilizadas

### Backend
- Node.js
- Express.js
- SQLite
- Body-parser
- CORS

### Frontend
- React.js
- React Router
- Axios

## Funcionalidades

- **Login de Usuário**: Permite aos usuários fazer login com nome e idade.
- **Adicionar Tarefas**: Permite adicionar novas tarefas à lista.
- **Visualizar Tarefas**: Exibe todas as tarefas do usuário logado.
- **Atualizar Tarefas**: Permite editar o texto das tarefas existentes.
- **Excluir Tarefas**: Permite excluir tarefas da lista.

## Instalação

### Pré-requisitos
- Node.js e npm instalados na máquina.
-React.js

### Backend

1. Navegue até o diretório `/backend`.
   cd backend
2. Instale as dependências.
    npm install
3. Inicie o servidor.
    node index.js
O servidor será iniciado em http://localhost:3001.

### Frontend
Navegue até o diretório /frontend.
   cd frontend
Instale as dependências.
   npm install
Inicie a aplicação.
   npm start
A aplicação será iniciada em http://localhost:3000.

### Utilização
Abra o navegador e acesse http://localhost:3000 para acessar a página de login.
Preencha o nome e a idade e clique no botão "Login".
Após o login bem-sucedido, você será redirecionado para a página de lista de tarefas.
Na página de lista de tarefas, você pode:
Adicionar uma nova tarefa digitando-a no campo de texto e clicando no botão "Add Task".
Atualizar uma tarefa clicando no campo de texto da tarefa e fazendo as alterações desejadas.
Excluir uma tarefa clicando no botão "Delete" ao lado dela.

### Estrutura do Projeto
/TODO-APP
├── /backend
│   ├── /node_modules
│   ├── database.db
│   ├── index.js
│   ├── package-lock.json
│   ├── package.json
├── /frontend
│   ├── /node_modules
│   ├── /public
│   ├── /src
│   │   ├── /components
│   │   │   ├── Login.js
│   │   │   ├── TodoList.js
│   │   ├── App.css
│   │   ├── App.js
│   ├── package-lock.json
│   ├── package.json
│   ├── README.md


### Backend
index.js: Configuração do servidor e rotas da API.
database.db: Banco de dados SQLite.

### Frontend
Login.js: Componente de login.
TodoList.js: Componente de lista de tarefas.
App.js: Configuração das rotas do React.
App.css: Estilos da aplicação.

### API Endpoints
### Autenticação

POST /login

Corpo da requisição: { "name": "string", "age": number }
Resposta: { "userId": number }

### Tarefas
GET /todos

Parâmetros: userId
Resposta: [ { "id": number, "userId": number, "task": "string" } ]
POST /todos

Corpo da requisição: { "userId": number, "task": "string" }
Resposta: { "id": number }
PUT /todos/:id

Corpo da requisição: { "task": "string" }
Resposta: { "changed": number }
DELETE /todos/:id

Resposta: { "deleted": number }

### Conclusão
Este projeto fornece uma base sólida para uma aplicação de lista de tarefas, demonstrando a integração entre um backend Node.js e um frontend React.js. Ele pode ser expandido para incluir funcionalidades adicionais, como autenticação mais robusta, validação de dados e uma interface de usuário mais avançada. Sinta-se à vontade para clonar o repositório, explorar o código e fazer melhorias!

   
