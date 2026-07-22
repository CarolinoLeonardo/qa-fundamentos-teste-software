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

# Estados do ciclo de vida do bug

## Novo/Aberto

É o primeiro estado do bug.

O bug entra nesse status quando o testador encontra uma falha e registra o problema na ferramenta de gestão.

Nesse momento, o bug ainda precisa ser analisado, priorizado e encaminhado para o responsável.

## Atribuído

O bug passa para o status **Atribuído** quando uma pessoa responsável é definida para investigar e corrigir o problema.

Normalmente, esse responsável será um desenvolvedor ou alguém do time técnico.

## Corrigido

O status **Corrigido** indica que o desenvolvedor realizou uma alteração no sistema para resolver o defeito.

Porém, nesse momento, o bug ainda não deve ser considerado finalizado.

Ele precisa voltar para o QA realizar o reteste.

## Testar

O status **Testar** indica que o bug corrigido precisa ser validado novamente pelo QA.

Nesta etapa, o testador executa os passos de reprodução novamente para confirmar se o problema foi realmente resolvido.

Também é importante observar se a correção não gerou novos problemas em outras partes do sistema.

## Fechado

O bug é marcado como **Fechado** quando o QA confirma que a correção funcionou corretamente.

Esse status indica que o problema foi resolvido e não precisa mais de ação.

## Reaberto

O bug é marcado como **Reaberto** quando a correção não resolveu o problema ou quando o mesmo comportamento volta a acontecer.

Nesse caso, o bug retorna para análise e correção.

---

# Exemplo prático

Imagine que um usuário tenta fazer login no sistema e recebe um erro inesperado.

O fluxo poderia acontecer assim:

| Etapa       | Situação                                           |
| ----------- | -------------------------------------------------- |
| Novo/Aberto | O QA encontra o erro e registra o bug              |
| Atribuído   | O bug é encaminhado para um desenvolvedor          |
| Corrigido   | O desenvolvedor corrige o problema                 |
| Testar      | O QA realiza o reteste da funcionalidade           |
| Fechado     | O QA confirma que o login voltou a funcionar       |
| Reaberto    | Caso o erro continue acontecendo, o bug é reaberto |

---

# Exemplo de bug no ciclo de vida

**Título:** Erro inesperado 500 ao realizar login

**Status inicial:** Novo/Aberto

## Descrição

Ao tentar realizar login com usuário e senha válidos, o sistema retorna erro 500.

## Passos para reprodução

1. Acessar a tela de login.
2. Informar usuário válido.
3. Informar senha válida.
4. Clicar no botão **"Entrar"**.

## Resultado real

O sistema retorna erro 500.

## Resultado esperado

O sistema deve validar as credenciais e permitir o acesso do usuário.

## Após análise

O bug é atribuído ao desenvolvedor responsável.

## Após correção

O bug é marcado como **Corrigido**.

## Após reteste

Se o login funcionar corretamente, o bug é **Fechado**.

Se o erro continuar, o bug é **Reaberto**.

---

# Relação com o trabalho de QA

O QA participa diretamente de várias etapas do ciclo de vida do bug.

Entre suas responsabilidades estão:

* Identificar falhas.
* Registrar bugs.
* Escrever reports claros.
* Anexar evidências.
* Validar correções.
* Realizar retestes.
* Reabrir bugs quando necessário.
* Fechar bugs quando a correção for validada.

---

# Importância do ciclo de vida do bug

O ciclo de vida do bug ajuda o time a manter organização e rastreabilidade sobre os problemas encontrados.

Ele permite saber:

* Quais bugs ainda estão abertos.
* Quem está responsável por cada correção.
* Quais bugs já foram corrigidos.
* Quais bugs precisam ser retestados.
* Quais bugs foram fechados.
* Quais bugs voltaram a apresentar problemas.

---

# Conclusão

Nesta etapa, aprendi que encontrar um bug é apenas o começo do processo.

Para que o problema seja realmente resolvido, ele precisa passar por um fluxo organizado de registro, atribuição, correção, reteste e fechamento.

Esse controle é essencial para garantir a qualidade do software e evitar que falhas cheguem ao usuário final.

## Evidência de estudo

![Ciclo de vida do bug](https://github.com/CarolinoLeonardo/qa-fundamentos-teste-software/blob/main/images/ciblo_bug1.jpeg)

## Status

✅ Concluído.

