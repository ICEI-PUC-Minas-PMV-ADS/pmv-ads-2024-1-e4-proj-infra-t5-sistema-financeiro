# Especificações do Projeto

**Pré-requisitos:** [Documentação de Contexto](1-Documentação de Contexto.md)

## Personas

### João Silva

João Silva tem 35 anos, é um empreendedor que administra sua própria empresa de consultoria financeira. Ele precisa de uma solução que o ajude a gerenciar as finanças da empresa de forma eficiente e segura.

## Histórias de Usuários

| EU COMO... | QUERO/PRECISO... | PARA... |
|------------|-------------------|---------|
| Usuário do sistema | Registrar despesas | Manter um registro das transações financeiras |
| Administrador | Gerar relatórios financeiros | Analisar o desempenho financeiro da empresa |

## Modelagem do Processo de Negócio

### Análise da Situação Atual

Atualmente, as despesas da empresa são registradas manualmente em planilhas eletrônicas, o que torna difícil acompanhar todas as transações.

### Descrição Geral da Proposta

A proposta é desenvolver uma aplicação web e mobile que permita aos usuários registrar e gerenciar suas despesas de forma eficiente e segura.

### Processo 1 – Registro de Despesas

Este processo envolve o registro de despesas no sistema.

![Processo de Registro de Despesas](img/registro_despesas.png)

### Processo 2 – Geração de Relatórios Financeiros

Este processo envolve a geração de relatórios financeiros para análise.

![Processo de Geração de Relatórios](img/geracao_relatorios.png)

## Tabelas do Banco de Dados

### Despesa

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único da despesa |
| Valor | Decimal | Valor da despesa |
| Data  | Date | Data da despesa |

### Categoria

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único da categoria |
| Nome  | Varchar | Nome da categoria |

### SistemaFinanceiro

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único do sistema financeiro |
| Nome  | Varchar | Nome do sistema financeiro |

### UsuarioSistemaFinanceiro

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único do usuário no sistema financeiro |
| Nome  | Varchar | Nome do usuário |
| Email | Varchar | Email do usuário |
| Senha | Varchar | Senha do usuário (criptografada) |

### Compra

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único da compra |
| Valor | Decimal | Valor total da compra |
| Data  | Date | Data da compra |

### ItemCompra

| Campo | Tipo | Descrição |
|-------|------|-----------|
| ID    | Int  | Identificador único do item da compra |
| Nome  | Varchar | Nome do item |
| Quantidade | Int | Quantidade do item |
| PrecoUnitario | Decimal | Preço unitário do item |

## Indicadores de Desempenho

Os principais indicadores de desempenho incluem o total de despesas registradas, o tempo médio de geração de relatórios e a satisfação do usuário.

## Requisitos
# Requisitos

## Requisitos Funcionais (RF)

| ID    | Descrição do Requisito                      | Prioridade |
|-------|---------------------------------------------|------------|
| RF-001| Permitir o registro de despesas             | Alta       |
| RF-002| Possibilitar a geração de relatórios financeiros | Alta |
| RF-003| Permitir o cadastro de categorias de despesas | Média   |
| RF-004| Implementar autenticação de usuários        | Alta       |
| RF-005| Garantir o armazenamento seguro das senhas  | Alta       |

## Requisitos Não Funcionais (RNF)

| ID    | Descrição do Requisito                                       | Prioridade |
|-------|--------------------------------------------------------------|------------|
| RNF-001| O sistema deve ser responsivo e compatível com dispositivos móveis | Alta |
| RNF-002| Garantir que a aplicação seja intuitiva e fácil de usar     | Média      |
| RNF-003| As transações financeiras devem ser processadas em tempo real | Alta    |
| RNF-004| O sistema deve ser compatível com múltiplos navegadores     | Alta      |

# Restrições

O projeto está restrito pelos seguintes itens:

| ID    | Restrição                                      |
|-------|------------------------------------------------|
| R-001 | Disponibilidade de recursos financeiros       |
| R-002 | Prazo de entrega do projeto                   |
| R-003 | Tecnologias previamente definidas             |

# Diagrama de Casos de Uso

Os casos de uso especificam a interação entre o usuário e o sistema. Abaixo está o diagrama de casos de uso para o sistema financeiro:

![Diagrama de Casos de Uso](img/diagrama_casos_uso.png)

# Matriz de Rastreabilidade

A matriz de rastreabilidade é uma ferramenta utilizada para rastrear os requisitos do sistema em diferentes artefatos do projeto. Abaixo está uma representação simplificada da matriz de rastreabilidade:

![Matriz de Rastreabilidade](img/matriz_rastreabilidade.png)

# Gerenciamento de Projeto

## Gerenciamento de Tempo

Para o gerenciamento de tempo, utilizaremos o diagrama de Gantt para visualizar as tarefas e seu cronograma:

![Diagrama de Gantt](img/diagrama_gantt.png)

## Gerenciamento de Equipe

O gerenciamento de equipe será feito por meio de uma ferramenta de gestão de tarefas, que permitirá atribuir atividades aos membros da equipe e acompanhar seu progresso.

## Gestão de Orçamento

A gestão de orçamento será realizada considerando os recursos financeiros disponíveis e os custos estimados para cada fase do projeto.


