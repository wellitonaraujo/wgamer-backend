# wgamer-backend

## WGAMER API
A WGAMER API é uma aplicação Node.js que fornece serviços para gerenciar categorias e produtos relacionados a jogos. A API inclui autenticação JWT para proteger rotas privadas e oferece funcionalidades para criar, editar, listar e excluir produtos, bem como gerenciar categorias.

## Pré-requisitos
Antes de iniciar, certifique-se de ter as seguintes ferramentas instaladas:

- Node.js (versão 14 ou superior)
- Yarn
- PostgresSQL
- Um arquivo .env configurado (veja as instruções abaixo)

#### PORT: A porta em que a API será executada.
#### DATABASE_URL: A URL de conexão com o banco de dados PostgresSQL.
#### JWT_SECRET: A chave secreta usada para assinar tokens JWT.

# Instalação
Clone este repositório:

- git clone https://github.com/wellitonaraujo/wgamer-backend.git
- Navegue até o diretório do projeto:
- cd wgamer-backend:
- Instale as dependências usando o Yarn:
- yarn install:

# Uso
Para executar a API, use o seguinte comando:

- yarn dev
#### A API estará acessível em http://localhost:3333 por padrão.

# Rotas
### Autenticação
- POST /auth: Cria um novo usuário.
- POST /session: Autentica um usuário e gera um token JWT.
### Categorias
- POST /category: Cria uma nova categoria.
- GET /category: Lista todas as categorias.
### Produtos
- POST /products: Cria um novo produto.
- GET /products: Lista todos os produtos.
- GET /products/:id: Obtém detalhes de um produto específico.
- PUT /products/:id: Atualiza um produto.
- DELETE /products/:id: Exclui um produto.

# Proteção de Rotas
#### As rotas para criar, atualizar, ver e apagar produtos são protegidas e requerem autenticação. Certifique-se de incluir o token JWT no cabeçalho de autorização das solicitações.

### Contribuição
Sinta-se à vontade para contribuir para este projeto. Se você tiver sugestões de melhorias ou encontrar problemas, abra uma issue ou envie uma pull request.
