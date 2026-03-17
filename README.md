# Gestão Financeira e Controle de Fluxo de Caixa

### Objetivo do Projeto

Este projeto foi desenvolvido para suprir a necessidade de uma gestão financeira centralizada e automatizada. O objetivo principal é monitorar a saúde do negócio através do controle rigoroso de entradas e saídas, permitindo a análise da rentabilidade real e da liquidez imediata.

### Desenvolvimento Técnico
A robustez da planilha foi garantida através de funções que automatizam o processamento de dados e previnem erros de visualização:

Agregação Condicional (SOMASE): Utilizada para consolidar fluxos financeiros por categoria. Esta lógica permite que o dashboard separe automaticamente o que é receita bruta do que são custos operacionais.

Aplicação: =SOMASE([@Tipo];"Saída";[@Valor])

Tratamento de Exceções (SEERRO): Implementada para manter a integridade dos indicadores de performance (KPIs). Isso evita que divisões por zero ou períodos sem dados "quebrem" o visual do dashboard, mantendo uma apresentação impecável.

Aplicação: =SEERRO([@[Saldo Líquido em Caixa]]/[@[Faturamento Total (Entradas)]];0)

Tabelas Inteligentes: A estrutura de dados foi montada para ser escalável, onde novos lançamentos são automaticamente incorporados aos cálculos e gráficos sem necessidade de intervenção manual.

<img width="751" height="464" alt="Captura de tela 2026-03-16 213723" src="https://github.com/user-attachments/assets/a760bba0-8c0c-4a80-81c5-feea37ea2635" />

![dash_financeiro_excel](https://github.com/user-attachments/assets/ff6cae77-c9e9-44a1-b54a-d159eb107a17)

### Explicação Estratégica do Dashboard
O painel visual foi desenhado seguindo princípios de Business Intelligence, priorizando os indicadores que realmente movem o ponteiro do negócio.

I. Indicadores de Performance (KPIs)
Faturamento Total (Entradas): Visibilidade total da receita bruta captada.

Saldo Líquido em Caixa: O principal indicador de liquidez, mostrando o valor real disponível após a dedução de todas as saídas.

Margem Líquida (%): Através do gráfico de rosca, monitoramos a eficiência da operação. No cenário atual, a margem de 39% indica uma operação saudável com boa retenção de lucro.

II. Análise Temporal de Fluxos
Evolução Mensal (Entradas vs. Saídas): O gráfico de barras permite identificar o comportamento sazonal do caixa. É possível visualizar rapidamente meses onde o custo operacional subiu e comparar se o faturamento acompanhou esse crescimento.

Saldo Mensal: Uma linha de tendência que ajuda a prever se o negócio está acumulando capital ou queimando caixa ao longo do tempo.

<img width="683" height="384" alt="Captura de tela 2026-03-16 214855" src="https://github.com/user-attachments/assets/cf7233ec-16c3-4aad-b24c-bccf2ae192a0" />

### Impacto de Negócio

A implementação deste sistema de controle transforma registros contábeis em Inteligência de Mercado. Com este projeto, é possível:

Identificar Sazonalidade: Planejar reservas financeiras para meses de maior pressão sobre o caixa.

Tomar Decisões Data-Driven: Avaliar se a empresa tem fôlego para novos investimentos baseando-se na margem líquida real.

Garantir Integridade: O uso de fórmulas de tratamento de erro garante que a gestão sempre tome decisões baseadas em números precisos e visuais limpos.
