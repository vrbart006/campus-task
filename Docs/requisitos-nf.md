# Requisitos Não Funcionais de Qualidade

## RNF-01 — Usabilidade
O sistema deve permitir que o usuário registre uma nova tarefa em no máximo 3 interações na interface.
→ Critério: testes com 5 usuários comprovam conclusão em até 3 toques.

## RNF-02 — Usabilidade
Mensagens de erro em linguagem simples, sem termos técnicos.
→ Critério: 100% compreendidas em testes com usuários.

## RNF-03 — Confiabilidade
Nenhuma informação deve ser perdida em caso de fechamento inesperado do aplicativo.
→ Critério: 10 simulações de crash sem perda de dados.

## RNF-04 — Segurança
Dados armazenados em área privada, inacessível a outros apps.
→ Critério: auditoria técnica de armazenamento confirma isolamento.

## RNF-05 — Eficiência de Desempenho
Carregamento da lista de tarefas em menos de 1 segundo em dispositivos com até 2 GB de RAM.
→ Critério: tempo médio inferior a 1000ms em 95% das execuções.

## RNF-06 — Eficiência de Desempenho
Consumo máximo de 50 MB de RAM com 200 tarefas ativas.
→ Critério: monitoramento em sessão de 15 minutos não supera 50 MB.

## RNF-07 — Manutenibilidade
Código organizado em módulos independentes por funcionalidade.
→ Critério: menos de 2 dependências diretas por módulo.