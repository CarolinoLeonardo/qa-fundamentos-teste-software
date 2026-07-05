# 10 - Ciclo de Vida do Bug

Esta pasta documenta meus estudos sobre o ciclo de vida de um bug dentro do processo de desenvolvimento e teste de software.

Nesta etapa, compreendi que um bug não termina quando é encontrado. Ele precisa ser registrado, analisado, corrigido, retestado e somente então fechado.

## Objetivo desta etapa

O objetivo deste módulo foi entender como um bug é gerenciado desde sua abertura até seu fechamento, passando por diferentes estados dentro de uma ferramenta de gestão de bugs.

## O que é o ciclo de vida do bug?

O ciclo de vida do bug representa os possíveis estados pelos quais um defeito passa após ser identificado durante os testes.

Esse processo normalmente é controlado por ferramentas de gestão de bugs, também chamadas de:

- Bugtrackers.
- Issue trackers.
- Ferramentas de gestão de tarefas.
- Ferramentas de gestão de defeitos.

Exemplos de ferramentas que podem ser usadas nesse processo:

- Jira.
- Azure DevOps.
- GitHub Issues.
- GitLab Issues.
- Trello.
- Bugzilla.
- Redmine.

## Fluxo estudado

O ciclo de vida padrão estudado possui o seguinte fluxo:

```md
Novo/Aberto → Atribuído → Corrigido → Testar → Fechado
                                      ↓
                                   Reaberto
                                      ↓
                                  Atribuído
```
