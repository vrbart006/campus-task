# Decisões de Engenharia

## Arquitetura Geral
Arquitetura em camadas: Presentation → Business Logic → Data

- Operações de banco em threads secundárias (async/await)
- Meta: 60 fps durante navegação
- Padrão Repository para persistência

## Interface (Usabilidade)
- Bottom Navigation Bar com 3 rotas principais
- Modal bottom sheet para criação de tarefa em até 3 toques
- Componentes com suporte WCAG AA (contraste mínimo)
- Textos de erro centralizados em constants/

## Persistência (Confiabilidade)
- SQLite com transações atômicas
- Escrita confirmada antes de atualizar a UI
- Repository Pattern centraliza lógica de dados

## Segurança
- Android Internal Storage / iOS App Sandbox
- Sem transmissão de dados a servidores externos (v1)
- Diretório privado do aplicativo

## Performance
- Paginação: 20 itens por vez
- Índice no campo data_vencimento
- Consultas incrementais (sem full table scan)

## Manutenibilidade
- Estrutura: features/tasks/, features/notifications/
- Injeção de dependência para desacoplamento
- Cobertura mínima de testes: 70% por módulo