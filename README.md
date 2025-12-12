# Thera Consulting - Sistema de Gerenciamento de Produtos

Este repositório contém os links para os projetos de teste de desenvolvimento (Frontend e Backend) para o sistema de gerenciamento de produtos.

## 📋 Estrutura do Projeto

O projeto está dividido em dois repositórios separados:

### 🎨 Frontend Test
- **Repositório**: [https://github.com/samoutinho/frontend-test](https://github.com/samoutinho/frontend-test)
- **Tecnologias**: Next.js, TypeScript, Zustand, Tailwind CSS, MSW
- **Descrição**: Aplicação web para gerenciamento de produtos com foco em interface moderna e responsiva
- **Status**: ✅ Implementado com todas as funcionalidades obrigatórias e extras

### ⚙️ Backend Test
- **Repositório**: [https://github.com/samoutinho/backend-test](https://github.com/samoutinho/backend-test)
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

## 🆕 Últimas Implementações

### Backend
- ✅ **Campo imagem em produtos**: Suporte a URLs de imagens externas
- ✅ **Migration de imagem**: Migration criada e executada para adicionar coluna `imagem` na tabela `products`
- ✅ **Paginação server-side**: Endpoint de produtos com suporte a `page` e `limit` como query parameters

### Frontend
- ✅ **Máscara de preço**: Formatação automática de preço durante digitação (R$ 1.234,56)
- ✅ **Imagens externas**: Suporte a URLs de imagens da internet (configurado no Next.js)
- ✅ **Melhorias de UX**: Correção de cores dos campos do formulário para melhor visibilidade
- ✅ **Paginação integrada**: Paginação client-side integrada com backend

### Documentação
- ✅ **Snapshots de tela**: Imagens de teste do Playwright adicionadas na pasta `screenshots/`
- ✅ **README atualizado**: Documentação completa das novas funcionalidades

## 📸 Snapshots de Tela

Este repositório contém snapshots de tela gerados durante os testes automatizados com Playwright. As imagens estão disponíveis na pasta `screenshots/` e documentam o estado visual da aplicação em diferentes momentos do desenvolvimento:

- **Testes de funcionalidades**: Capturas das telas principais (listagem de produtos, formulários, etc.)
- **Testes de integração**: Verificação visual de componentes e layouts
- **Validação de UI**: Garantia de que a interface não quebra após alterações

Esses snapshots servem como referência visual e podem ser usados para:
- Documentação visual da aplicação
- Comparação antes/depois de alterações
- Validação de regressões visuais
- Referência para novos desenvolvedores

## 📄 Licença

Este projeto é público e está disponível para fins de avaliação técnica.

