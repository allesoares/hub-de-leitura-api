# 📚 Hub de Leitura API - Sistema de Biblioteca para QA


**API educacional completa para aprendizado e prática de Quality Assurance (QA)**

##Json do postman##



![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)
![Express](https://img.shields.io/badge/Express-4.18+-blue.svg)
![SQLite](https://img.shields.io/badge/SQLite-3+-lightgrey.svg)
![JWT](https://img.shields.io/badge/JWT-Auth-orange.svg)
![License](https://img.shields.io/badge/License-Educational-yellow.svg)

## 🎯 Objetivo

O **Hub de Leitura API** é uma API REST de gestão de biblioteca desenvolvida especificamente para **ensinar e praticar Quality Assurance**. Cada endpoint representa cenários reais que profissionais de QA encontram no dia a dia.

### 🎓 Para Estudantes de QA

- ✅ **Aprenda testando** - API real com cenários complexos
- ✅ **API REST completa** - Todos os tipos de endpoint
- ✅ **Diferentes perfis** - Usuário comum vs Administrador
- ✅ **Autenticação JWT** - Sistema de login profissional
- ✅ **Cenários de erro** - Como APIs falham na prática
- ✅ **Documentação Swagger** - API bem documentada

## 🚀 Funcionalidades da API

### 👤 **Gestão de Usuários**

- Registro e login de usuários
- Autenticação JWT com expiração
- Perfis diferenciados (Usuário/Admin)
- Atualização de perfil

### 📖 **Catálogo de Livros**

- Listagem com filtros e busca
- CRUD completo (Admin)
- Controle de estoque
- Upload de capas
- Categorização

### 📝 **Reservas**

- Reserva de livros disponíveis
- Controle de prazos
- Gestão de retiradas e devoluções
- Histórico completo
- Alertas de atraso

### 🛠️ **Administração**

- Dashboard com estatísticas
- Gestão de todas as reservas
- Controle de usuários
- Relatórios e exportações
- Logs do sistema

## 🛠️ Tecnologias

- **Node.js** - Runtime JavaScript
- **Express.js** - Framework web
- **SQLite** - Banco de dados leve
- **JWT** - Autenticação
- **Bcrypt** - Criptografia de senhas
- **Joi** - Validação de dados
- **Swagger** - Documentação da API

## ⚡ Instalação Rápida

### Pré-requisitos

- Node.js 18+ instalado
- Git instalado

### 1. Clone o Repositório

```bash
git clone https://github.com/EBAC-QE/hub-de-leitura-api.git
cd hub-de-leitura-api
```

### 2. Instale as Dependências

```bash
npm install
```

### 3. Inicie o Servidor

```bash
npm start
```

### 4. Acesse a Documentação

- **API Docs:** http://localhost:3000/api-docs

## 🔑 Credenciais de Teste

### Administrador

- **Email:** admin@biblioteca.com
- **Senha:** admin123
- **Permissões:** Acesso total ao sistema

### Usuário Comum

- **Email:** usuario@teste.com
- **Senha:** user123
- **Permissões:** Reservas e consultas

## 🧪 Testando a API

### Com cURL

```bash
# Login
curl -X POST http://localhost:3000/api/login \
  -H "Content-Type: application/json" \
  -d '{"email":"admin@biblioteca.com","password":"admin123"}'

# Listar livros (com token)
curl -X GET http://localhost:3000/api/books \
  -H "Authorization: Bearer SEU_TOKEN_AQUI"
```

### Com Postman/Insomnia

1. Importe a coleção do Swagger: http://localhost:3000/api-docs
2. Configure o token JWT no cabeçalho Authorization
3. Teste todos os endpoints disponíveis

## 🤝 Contribuindo

### Para Instrutores

1. Fork o repositório
2. Crie cenários de teste adicionais
3. Adicione novos endpoints para prática
4. Documente bugs intencionais para os alunos encontrarem
5. Envie um Pull Request

### Para Alunos

1. Reporte bugs encontrados (é parte do aprendizado!)
2. Sugira melhorias na documentação
3. Compartilhe casos de teste interessantes
4. Contribua com exemplos de automação

### Resetar Banco de Dados

```bash
# Pare o servidor "CTRL + C" e delete o arquivo do banco
rm database/biblioteca.db
# Rode o comando para recriar o banco
npm run db
# Reinicie o servidor para recriar as tabelas
npm start
```

## 🐛 Problemas Comuns

### Erro "Port 3000 already in use"

```bash
# Rode numa porta diferente, por exemplo, porta 3001
PORT=3001 npm start
```

### Token expirado

- Faça login novamente para obter um novo token
- Tokens expiram em 1 hora por padrão

### Banco de dados corrompido

- Delete o arquivo `database/biblioteca.db`
- Rode o comando `npm run db` para recriar o banco

## 📚 Recursos de Aprendizado

### Documentação

- [Express.js](https://expressjs.com/)
- [JWT.io](https://jwt.io/)
- [SQLite Tutorial](https://www.sqlitetutorial.net/)
- [Swagger/OpenAPI](https://swagger.io/docs/)

### Ferramentas de Teste

- [Postman](https://www.postman.com/)
- [Insomnia](https://insomnia.rest/)
- [Jest](https://jestjs.io/) - Para testes automatizados
- [Newman](https://github.com/postmanlabs/newman) - CLI do Postman

### Uso Permitido

- ✅ Uso educacional e acadêmico
- ✅ Modificação para fins didáticos
- ✅ Distribuição para alunos
- ✅ Criação de cursos baseados no projeto

### Uso Restrito

- ❌ Uso comercial direto
- ❌ Venda do código
- ❌ Redistribuição sem créditos

---

## ⭐ Agradecimentos

Desenvolvido com ❤️ para a comunidade de **Quality Assurance**.

**Contribuidores:**

- Fábio Araújo
   - [Repositório](https://github.com/fabioaraujoqa)
   - [Linkedin](https://www.linkedin.com/in/fabio10/)

---

### 🚀 **Bons Testes!**

*"A qualidade nunca é um acidente; ela é sempre o resultado de um esforço inteligente."* - John Ruskin
