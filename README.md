# 🚀 OrderFlow API

Backend da plataforma **OrderFlow**, desenvolvido com Node.js, Express e PostgreSQL para gerenciamento de pedidos online.

A API fornece autenticação de usuários, gerenciamento de produtos, categorias, pedidos e integração com pagamentos via Stripe.

---

![Node.js](https://img.shields.io/badge/Node.js-20.x-green)

![Express](https://img.shields.io/badge/Express-5.x-black)

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue)

![JWT](https://img.shields.io/badge/Auth-JWT-orange)

![Stripe](https://img.shields.io/badge/Payments-Stripe-purple)

Backend da plataforma...

## 📌 Funcionalidades

- ✅ Autenticação JWT
- ✅ Cadastro de usuários
- ✅ Controle de acesso (Administrador e Cliente)
- ✅ CRUD de Produtos
- ✅ CRUD de Categorias
- ✅ Upload de imagens com Multer
- ✅ Gerenciamento de Pedidos
- ✅ Atualização do status dos pedidos
- ✅ Integração com Stripe
- ✅ API REST

---

## 🛠 Tecnologias

- Node.js
- Express
- PostgreSQL
- Sequelize
- JWT
- Multer
- Stripe
- Bcrypt
- Yup
- Cors

---

## 📂 Estrutura do Projeto

```
src
├── app
│   ├── controllers
│   ├── models
│   ├── middlewares
│   ├── schemas
│   └── config
│
├── database
│   ├── migrations
│   └── seeders
│
├── routes
│
└── server.js
```

---

## 🔐 Autenticação

A autenticação é realizada utilizando **JWT (JSON Web Token)**.

Após realizar o login, o token deve ser enviado no Header das requisições protegidas.

```
Authorization: Bearer seu_token
```

---

## 📦 Principais Endpoints

### Usuários

| Método | Endpoint | Descrição |
|---------|----------|-----------|
| POST | /users | Criar usuário |
| POST | /session | Login |

---

### Produtos

| Método | Endpoint |
|---------|----------|
| GET | /products |
| POST | /products |
| PUT | /products/:id |
| DELETE | /products/:id |

---

### Categorias

| Método | Endpoint |
|---------|----------|
| GET | /categories |
| POST | /categories |

---

### Pedidos

| Método | Endpoint |
|---------|----------|
| GET | /orders |
| POST | /orders |
| PUT | /orders/:id |

---

## ⚙️ Instalação

Clone o projeto

```bash
git clone https://github.com/carloshenrique2026/orderflow-api.git
```

Entre na pasta

```bash
cd orderflow-api
```

Instale as dependências

```bash
npm install
```

Configure as variáveis de ambiente

```env
DATABASE_URL=

JWT_SECRET=

STRIPE_SECRET_KEY=
```

Execute as migrations

```bash
npx sequelize db:migrate
```

Inicie o servidor

```bash
npm run dev
```

---

## 🧪 Testes

As requisições podem ser testadas utilizando:

- Postman
- Insomnia

---

## 🚧 Próximas Melhorias

- [ ] Documentação Swagger
- [ ] Docker
- [ ] Testes Automatizados
- [ ] CI/CD
- [ ] Rate Limiter
- [ ] Logs estruturados
- [ ] Paginação
- [ ] Cache com Redis

---

## 👨‍💻 Desenvolvedor

Carlos Henrique 

LinkedIn:
https://linkedin.com/in/carloshenrique2026

Portfólio:
https://carloshenriqueprogramador.com.br

Frontend:
https://github.com/carloshenrique2026/orderflow-web