# Thera Consulting - Sistema de Gerenciamento de Produtos

Este repositório contém os links para os projetos de teste de desenvolvimento (Frontend e Backend) para o sistema de gerenciamento de produtos.

## 📋 Estrutura do Projeto

O projeto está dividido em dois repositórios separados:

### 🎨 Frontend Test
- **Repositório**: [thera-consulting-frontend-test](./frontend-test)
- **Tecnologias**: Next.js, TypeScript, Zustand, Tailwind CSS, MSW
- **Descrição**: Aplicação web para gerenciamento de produtos com foco em interface moderna e responsiva
- **Status**: ✅ Implementado com todas as funcionalidades obrigatórias e extras

### ⚙️ Backend Test
- **Repositório**: [thera-consulting-backend-test](./backend-test)
- **Tecnologias**: NestJS, TypeScript, PostgreSQL, Clean Architecture, Docker
- **Descrição**: API RESTful para gerenciamento de produtos e pedidos seguindo princípios SOLID
- **Status**: ✅ Implementado com todas as funcionalidades obrigatórias e extras

## 🚀 Como Começar

Cada repositório possui suas próprias instruções de instalação e execução. Consulte os README.md específicos de cada projeto:

- [Instruções do Frontend](./frontend-test/README.md)
- [Instruções do Backend](./backend-test/README.md)

### Inicialização Rápida

**Backend (porta 3001):**
```bash
cd backend-test
docker-compose up -d
# ou
npm install && npm run start:dev
# Acesse: http://localhost:3001
# Swagger: http://localhost:3001/api
```

**Frontend (porta 3002):**
```bash
cd frontend-test
npm install && npm run dev
# Acesse: http://localhost:3002
```

**Nota**: As portas foram configuradas para evitar conflitos:
- Backend: porta 3001
- Frontend: porta 3002

## 📝 Objetivo

Desenvolver um sistema completo de gerenciamento de produtos demonstrando:
- Boas práticas de desenvolvimento
- Arquitetura limpa e organizada
- Testes automatizados
- Documentação completa
- Uso de tecnologias modernas

## 📄 Licença

Este projeto é público e está disponível para fins de avaliação técnica.

