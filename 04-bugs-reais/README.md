# 04 - Bugs Reais

Esta pasta documenta meus estudos sobre bugs reais que causaram grandes impactos em sistemas, empresas e usuários.

O objetivo desta etapa foi entender que falhas de software podem gerar prejuízos financeiros, riscos à segurança, perda de confiança e até consequências fatais.

## Objetivo do estudo

Compreender, por meio de exemplos reais, a importância dos testes de software e da identificação antecipada de falhas.

## Por que estudar bugs reais?

Estudar bugs reais ajuda a perceber que o teste de software não é apenas uma etapa técnica do desenvolvimento.

Ele tem impacto direto em:

- Segurança dos usuários.
- Reputação da empresa.
- Custos financeiros.
- Continuidade do negócio.
- Confiabilidade do produto.
- Tomada de decisão sobre uma entrega.

## Exemplos estudados

### Ônibus Espacial Challenger

O ônibus espacial Challenger explodiu 73 segundos após seu lançamento em 1986.

Além da perda estimada em bilhões de dólares, todos os 7 tripulantes morreram.

O acidente ocorreu devido à perda de elasticidade dos anéis de vedação, feitos de borracha, em uma temperatura mais baixa do que a considerada nos testes.

Segundo minhas anotações, a temperatura esperada nos testes era de aproximadamente 17°C, mas no lançamento estava próxima de 2°C.

Esse caso mostra a importância de testar sistemas considerando diferentes condições reais de uso.

## Boeing 737 MAX

A crise do Boeing 737 MAX envolveu dois acidentes que resultaram em 346 mortes e bilhões de dólares em prejuízo.

As quedas foram causadas por falhas no sistema MCAS, e a Boeing admitiu que já tinha conhecimento de problemas no software antes dos acidentes.

Esse caso reforça a importância de:

- Testes rigorosos em sistemas críticos.
- Comunicação clara sobre riscos.
- Validação de requisitos de segurança.
- Investigação adequada de falhas antes da liberação.

## Mars Climate Orbiter

A NASA perdeu a sonda espacial Mars Climate Orbiter quando ela entrava na atmosfera de Marte.

O problema ocorreu porque o software de navegação utilizava unidades métricas, enquanto outro software utilizava unidades imperiais, como milhas, jardas e pés.

Esse caso mostra como falhas de integração e comunicação entre sistemas podem causar grandes prejuízos.

## Bug no YouTube

O YouTube teve um bug de overflow quando um vídeo ultrapassou o limite de uma variável de 32 bits.

Esse exemplo mostra que até sistemas muito grandes podem ser afetados por limitações técnicas aparentemente simples.

## Relação com QA

Esses casos mostram que o profissional de QA precisa pensar além do “funciona ou não funciona”.

É necessário considerar:

- Cenários extremos.
- Regras de negócio.
- Integrações entre sistemas.
- Limitações técnicas.
- Impacto para o usuário.
- Riscos de produção.

## Conclusão

Estudar bugs reais reforçou minha percepção de que testes de software são essenciais para prevenir falhas graves.

Quanto maior o impacto de um sistema na vida das pessoas ou no funcionamento de uma empresa, maior deve ser o cuidado com planejamento, execução, documentação e análise dos testes.

## Evidência de estudo

![Anotações sobre bugs reais](../images/bugs-reais-01.jpeg)

## Status

Concluído.
