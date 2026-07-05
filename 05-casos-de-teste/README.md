# 05 - Casos de Teste

Esta pasta documenta meus estudos sobre casos de teste e suas diferentes formas de documentação.

Nesta etapa, estudei o conceito de caso de teste, scripts de teste, casos de teste padrão, cenários de teste e linguagem Gherkin.

## O que é um caso de teste?

De acordo com o glossário da Syllabus, um caso de teste é um conjunto de:

- Pré-condições.
- Entradas.
- Ações.
- Resultados esperados.
- Pós-condições.

Esses elementos são desenvolvidos com base nas condições de teste.

## Definição complementar

No livro *Systematic Software Testing*, o caso de teste descreve uma condição particular a ser testada.

Ele é composto por valores de entrada, restrições para execução e um resultado esperado.

## Objetivo dos casos de teste

Os casos de teste ajudam a documentar o que será verificado em um sistema.

Eles também servem para orientar a execução dos testes e garantir que o comportamento esperado seja validado de forma organizada.

## Scripts de Teste

O script de teste é uma forma mais detalhada de documentar um teste.

Geralmente, ele detalha linha por linha os dados e passos necessários para executar o teste.

Por exigir uma documentação mais rica, normalmente leva mais tempo para ser criado.

## Casos de Teste Padrão

Os casos de teste padrão descrevem uma ideia específica a ser testada, mas sem detalhar todos os dados e etapas exatas de execução.

Eles oferecem mais flexibilidade para o testador decidir como completar o teste.

Sua elaboração costuma ser mais rápida do que a criação de scripts de teste.

## Cenários de Teste

Os cenários de teste descrevem o objetivo do usuário no sistema.

Eles possuem poucas instruções de execução e dão grande flexibilidade ao testador.

Essa técnica é útil para mapear testes regressivos antes da automação, pois reduz o tempo de modelagem e libera mais tempo para o analista criar scripts automatizados.

## Diferença entre Script, Caso de Teste e Cenário de Teste

| Tipo | Característica principal | Nível de detalhe |
|---|---|---|
| Script de Teste | Descreve passo a passo como executar o teste | Alto |
| Caso de Teste Padrão | Descreve uma condição específica a ser testada | Médio |
| Cenário de Teste | Descreve o objetivo do usuário no sistema | Baixo |

## Linguagem Gherkin

A linguagem Gherkin tem como função padronizar a forma de descrever especificações de cenários com base nas regras de negócio.

Ela torna os testes mais fáceis de ler, inclusive por pessoas que não possuem conhecimento técnico.

A ideia é deixar a programação “por trás”, enquanto o código executa aquilo que o Gherkin descreve.

## Exemplo de estrutura em Gherkin

```gherkin
# language: pt

Funcionalidade: Autenticação de Login

Contexto:
Dado que eu desejo autenticar no sistema

Esquema do Cenário: Deve conseguir acessar o sistema
Quando eu informo um usuário "<usuario>" e uma senha "<senha>"
E clico no botão entrar
Então recebo a mensagem "<mensagem>"

Exemplos:
| usuario    | senha  | mensagem                                    |
| wag.torres | 123456 | Acesso realizado com sucesso.              |
| wag.torres | 123455 | Usuário ou senha inválidos                  |
| wag.torres | 123456 | Usuário bloqueado                           |
|            |        | Campo obrigatório: usuário; Campo obrigatório: senha |
