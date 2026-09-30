# Painel de Produção: aderência ao plano, OEE e paradas

Projeto de portfólio em análise de dados, desenvolvido em **Power BI**.
Os dados são **simulados** e não representam uma empresa real.

## Pergunta de negócio

Onde a produção perde eficiência e o que deve ser tratado primeiro?

O painel atende a gestores, ao PCP (Planejamento e Controle da Produção), à Manutenção e à Qualidade.

## O que o painel mostra

### Página Gestor
Visão geral da produção: aderência ao plano, OEE (eficiência global), produtividade, peças rejeitadas, comparativo entre 2025 e 2026 e Pareto das paradas não planejadas.

![Página Gestor](https://i.ibb.co/KzLVQXv3/Captura-de-tela-2026-09-29-181544.png)

### Dica de ferramenta
Ao passar o mouse sobre o gráfico de OEE, aparece o comparativo semanal (semana atual contra a semana anterior).

![Dica de ferramenta: comparativo semanal](https://i.ibb.co/mFRds4wc/Captura-de-tela-2026-09-29-181554.png)

### Página PCP e Manutenção
Mostra onde e quando ocorrem as perdas: aderência por linha e semana, planejado e realizado por linha, paradas por área responsável, por dia da semana e turno, e por linha.

![Página PCP e Manutenção](https://i.ibb.co/k2tC1ww8/Captura-de-tela-2026-09-29-181602.png)

### Página Conclusão
Reúne os achados, as causas prováveis, as recomendações e as limitações do estudo.

![Página Conclusão](https://i.ibb.co/whBvhfWY/Captura-de-tela-2026-09-29-181613.png)

## Principais achados

1. **Linha PIN-02, agosto de 2026:** a aderência ao plano foi de 84%, 69%, 62% e 73% nas semanas de 03 a 24/08 e voltou a cerca de 100% em setembro. As quebras de equipamento somaram 56,5 horas nessas quatro semanas, contra 212,5 horas nas outras 100 semanas.
2. **Linha MON-01:** o produto C tem 8,2% de peças rejeitadas, contra 2,5% nos demais produtos da linha.
3. **Sextas-feiras à tarde:** a falta de operador é de 0,47 hora por turno e por linha, contra 0,07 a 0,09 hora nos demais dias e turnos.
4. **Manutenção:** responde por cerca de 54% das horas paradas não planejadas.

## Indicadores

| Indicador | Valor | Como é calculado |
|---|---|---|
| Aderência ao plano | 98,7% | Peças aprovadas divididas pelas peças planejadas |
| OEE (eficiência global) | 74,0% | Disponibilidade × Performance × Qualidade |
| Disponibilidade | 83,4% | Horas produzidas divididas pelas horas programadas |
| Performance | 90,1% | Total produzido dividido pelo que seria produzido na velocidade ideal |
| Qualidade | 98,4% | Peças aprovadas divididas pelo total produzido |

## Dados e ferramentas

- Base simulada com 4 setores, 8 linhas de produção e 2 turnos, de 30/09/2024 a 25/09/2026 (104 semanas).
- Tabelas: Produção (7.968 registros), Paradas (24.478 registros), Calendário, Linha, Turno e Motivo.
- Conferência dos dados: as horas programadas menos as horas produzidas são iguais à soma das horas paradas (diferença zero).
- Ferramentas: Power BI (Power Query, modelagem de dados, medidas em DAX e visualização) e Excel.
- Os arquivos da base estão na pasta `dados`.

## Como abrir o painel

Baixe o arquivo `.pbix` e abra no Power BI Desktop, que é gratuito.
O resumo do projeto está no arquivo `Projeto_Painel_Producao_1_pagina.pdf`.

## Limitações

- Os dados são simulados: os resultados demonstram o método e não representam uma empresa real.
- As causas apontadas são hipóteses e precisam ser confirmadas na prática.
- O OEE considera como perda todas as paradas, inclusive as planejadas. Sem as paradas planejadas, o OEE seria de 81,0%.
- Não há metas oficiais nem custos: as faixas de cor e os prazos são sugestões da autora.

## Autora

**Gabriela Lima**
[LinkedIn](www.linkedin.com/in/gabriela-lima-dados)[Projeto_Painel_Producao.pdf](https://github.com/user-attachments/files/32833867/Projeto_Painel_Producao.pdf)
