# Cadastro de Produtos

Projeto Fullstack desenvolvido com Node.js, Express, MongoDB Atlas e JavaScript para gerenciamento de produtos.

## Funcionalidades

- Cadastrar produtos
- Listar produtos
- Buscar produto por ID
- Atualizar produtos
- Excluir produtos

## Estrutura

```text
src/
├── controllers/
│   ├── produtoController.js
│   └── userController.js
├── models/
│   ├── Produto.js
│   └── User.js
├── routes/
│   ├── produtoRoutes.js
│   └── userRoutes.js
└── server.js
```

## Executar o Projeto

### Backend

Instale as dependências:

```bash
npm install
```

Inicie o servidor:

```bash
npm start
```

Ou execute diretamente:

```bash
node src/server.js
```

O servidor ficará disponível em:

```text
http://localhost:3000
```

### Frontend

Abra o arquivo:

```text
front/index.html
```

Também é possível executar o frontend utilizando a extensão **Live Server** no Visual Studio Code.

## Banco de Dados

O projeto utiliza o MongoDB Atlas como banco de dados.

Crie um arquivo `.env` dentro da pasta do backend e informe as seguintes variáveis:

```env
MONGODB_URI=sua_string_de_conexao
PORT=3000
```

> Não envie o arquivo `.env` para o GitHub. Adicione esse arquivo ao `.gitignore`.

## Rotas da API

| Método | Rota | Ação |
|---|---|---|
| GET | `/produtos` | Lista todos os produtos |
| GET | `/produtos/:id` | Busca um produto pelo ID |
| POST | `/produtos` | Cadastra um produto |
| PUT | `/produtos/:id` | Atualiza um produto |
| DELETE | `/produtos/:id` | Remove um produto |

## Exemplo de Produto

```json
{
  "nome": "Celular",
  "preco": 3000,
  "estoque": 10,
  "categoria": "Informática"
}
```

## Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript
- Node.js
- Express
- MongoDB Atlas
- Mongoose
- PWA (Progressive Web App)

## Autora

**Rejane Ferreira de Mendonça**

Projeto desenvolvido para a disciplina de PWA Fullstack.