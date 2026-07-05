# 06 - Linguagem Gherkin

Esta pasta documenta meus estudos sobre a linguagem Gherkin e sua aplicação na escrita de cenários de teste.

Nesta etapa, compreendi que Gherkin é uma linguagem utilizada para descrever comportamentos esperados de um sistema de forma simples, padronizada e compreensível para pessoas técnicas e não técnicas.

## Objetivo desta etapa

O objetivo deste módulo foi entender como a linguagem Gherkin pode ser utilizada para documentar cenários de teste com base em regras de negócio e comportamentos esperados do sistema.

## O que é Gherkin?

Gherkin é uma linguagem desenvolvida para que humanos possam utilizar como forma de entendimento e compreensão das especificações levantadas a partir da perspectiva dos stakeholders.

Ela permite escrever cenários de teste de forma mais próxima da linguagem natural, facilitando a comunicação entre pessoas de negócio, QA, desenvolvimento e produto.

## Para que serve o Gherkin?

A linguagem Gherkin serve para padronizar a forma de descrever especificações de cenários com base nas regras de negócio.

Ela torna os testes mais fáceis de ler, inclusive por pessoas que não possuem conhecimento técnico.

A ideia é deixar a programação “por trás”, enquanto o código executa aquilo que o Gherkin descreve.

## Estrutura básica do Gherkin

A escrita em Gherkin geralmente utiliza palavras-chave como:

| Palavra-chave | Função |
|---|---|
| Funcionalidade | Define a funcionalidade que será descrita |
| Cenário | Define uma situação específica a ser validada |
| Dado | Define o contexto inicial |
| Quando | Define a ação executada pelo usuário ou sistema |
| Então | Define o resultado esperado |
| E | Complementa uma etapa anterior |
| Esquema do Cenário | Permite testar o mesmo cenário com diferentes dados |
| Exemplos | Lista os dados utilizados no esquema do cenário |

## Exemplo simples em Gherkin

```gherkin
# language: pt

Funcionalidade: Autenticação de Login

Cenário: Login com dados válidos
Dado que o usuário acessa a tela de login
Quando informa e-mail e senha válidos
E clica no botão Entrar
Então o sistema deve permitir o acesso

## Exemplo com Esquema do Cenário
# language: pt

Funcionalidade: Autenticação de Login

Contexto:
Dado que eu desejo autenticar no sistema

Esquema do Cenário: Deve conseguir acessar o sistema
Quando eu informo um usuário "<usuario>" e uma senha "<senha>"
E clico no botão entrar
Então recebo a mensagem "<mensagem>"

Exemplos:
| usuario    | senha  | mensagem                                      |
| wag.torres | 123456 | Acesso realizado com sucesso.                 |
| wag.torres | 123455 | Usuário ou senha inválidos                    |
| wag.torres | 123456 | Usuário bloqueado                             |
|            |        | Campo obrigatório: usuário e senha            |

# Gherkin não é BDD

Um ponto importante estudado foi que **Gherkin e BDD não são a mesma coisa**.

**Gherkin** é uma linguagem utilizada para escrever cenários de comportamento.

**BDD**, ou **Behavior-Driven Development**, é uma metodologia de desenvolvimento de software guiada por comportamento.

O BDD pode utilizar Gherkin como apoio, mas Gherkin sozinho não significa que um time está praticando BDD.

## Diferença entre Gherkin, BDD e Cucumber

| Conceito | Explicação                                                    |
| -------- | ------------------------------------------------------------- |
| Gherkin  | Linguagem usada para escrever cenários de forma compreensível |
| BDD      | Metodologia de desenvolvimento guiada por comportamento       |
| Cucumber | Ferramenta que pode executar cenários escritos em Gherkin     |

## Benefícios do uso do Gherkin

* Facilita a comunicação entre áreas técnicas e não técnicas.
* Aproxima regras de negócio da documentação de testes.
* Ajuda a transformar requisitos em cenários testáveis.
* Padroniza a escrita dos cenários.
* Pode servir como base para automação de testes.
* Torna a documentação mais clara e fácil de manter.

## Minha percepção

Nesta etapa, entendi que **Gherkin é uma ferramenta de comunicação**.

Mais do que escrever testes bonitos, o objetivo é garantir que todos entendam o comportamento esperado do sistema.

Também percebi que a linguagem Gherkin pode ajudar bastante na transição entre QA manual e automação, pois os cenários escritos de forma clara podem servir como base para testes automatizados no futuro.

## Evidência de estudo

![Gherkin e Ferramentas](https://github.com/CarolinoLeonardo/qa-fundamentos-teste-software/blob/main/images/gherkin_ferramentas1.jpeg)

## Status

✅ Concluído.

