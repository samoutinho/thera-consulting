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

- [Instruções do Frontend](https://github.com/samoutinho/frontend-test/blob/master/README.md)
- [Instruções do Backend](https://github.com/samoutinho/backend-test/blob/master/README.md)

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

## 🚧 Implementações Futuras

Este projeto foi desenvolvido como uma base sólida para evolução contínua. Abaixo estão as funcionalidades planejadas para futuras versões:

### Arquitetura e Infraestrutura
- **Multitenancy**: Suporte a múltiplos tenants/clientes com isolamento de dados
- **CI/CD Pipeline**: Automação de deploy e testes contínuos
- **Monitoramento e Observabilidade**: Integração com ferramentas de monitoramento (Prometheus, Grafana)
- **Cache e Performance**: Implementação de cache distribuído (Redis)
- **Rate Limiting**: Proteção contra abuso de API
- **Logs Estruturados**: Sistema de logging centralizado e estruturado

### Segurança e Autenticação
- **Reset de Senha**: Fluxo completo de recuperação de senha via email
- **Autenticação Multi-fator (MFA)**: Suporte a 2FA/TOTP
- **Gestão de Permissões**: Sistema de roles e permissões granulares (RBAC)
- **OAuth2/SSO**: Integração com provedores de autenticação externos
- **Auditoria**: Log de todas as ações críticas do sistema

### Melhorias de Dados
- **Categorias como Entidade**: Transformar categoria de texto livre para tabela auxiliar com relacionamentos
- **Tags e Etiquetas**: Sistema flexível de tags para produtos
- **Histórico de Alterações**: Versionamento de produtos e rastreamento de mudanças
- **Soft Delete**: Exclusão lógica de registros com possibilidade de recuperação

### Funcionalidades de Negócio
- **Carrinho de Compras**: Sistema completo de carrinho e checkout
- **Sistema de Avaliações**: Reviews e ratings de produtos
- **Notificações**: Sistema de notificações em tempo real (WebSockets)
- **Relatórios e Analytics**: Dashboard com métricas e relatórios gerenciais
- **Exportação de Dados**: Exportação em múltiplos formatos (CSV, Excel, PDF)
- **Importação em Lote**: Upload de produtos via arquivo CSV/Excel

### Experiência do Usuário
- **Upload de Imagens**: Upload direto de imagens ao invés de apenas URLs
- **Busca Avançada**: Busca full-text com filtros complexos
- **Filtros Salvos**: Salvar e reutilizar combinações de filtros
- **Tema Escuro/Claro**: Suporte a temas personalizáveis
- **Internacionalização (i18n)**: Suporte a múltiplos idiomas
- **PWA**: Transformar em Progressive Web App com suporte offline

### Qualidade e Testes
- **Testes E2E Abrangentes**: Cobertura completa com Playwright/Cypress
- **Testes de Performance**: Testes de carga e stress
- **Testes de Segurança**: Análise de vulnerabilidades automatizada
- **Cobertura de Testes**: Aumentar cobertura para >80%

### Integrações
- **Webhooks**: Sistema de webhooks para integrações externas
- **API GraphQL**: Adicionar endpoint GraphQL além de REST
- **Integração com Pagamentos**: Integração com gateways de pagamento
- **Integração com ERP**: Conectores para sistemas ERP populares
- **Integração com Marketplaces**: Sincronização com marketplaces (Mercado Livre, Amazon, etc.)

### Documentação
- **Documentação de API Interativa**: Melhorar documentação Swagger/OpenAPI
- **Guia de Contribuição**: Documentação para contribuidores
- **Changelog Automatizado**: Sistema de versionamento semântico
- **Tutoriais e Vídeos**: Material educativo para usuários

## 📄 Licença

Este projeto é público e está disponível para fins de avaliação técnica.

## 👤 Autor

**Samuel Alves Moutinho**

- 📧 Email: samuca.moutinho@gmail.com
- 🔗 GitHub: [@samoutinho](https://github.com/samoutinho)

Desenvolvido como parte do teste técnico para Thera Consulting.

