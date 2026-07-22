# 12 - Automação de Testes

Esta pasta documenta meus estudos sobre automação de testes de software.

Este foi o último capítulo do curso de Fundamentos de Teste de Software. Nesta etapa, compreendi que a automação de testes exige um esforço inicial maior, mas pode trazer grandes benefícios para a equipe no médio e longo prazo.

## Objetivo desta etapa

O objetivo deste módulo foi entender o papel da automação de testes, seus principais benefícios e também alguns cuidados importantes para evitar erros comuns durante sua implementação.

Os principais pontos estudados foram:

- O que é automação de testes.
- Benefícios da automação.
- Quando automatizar.
- O que evitar na automação.
- Limitações de ferramentas de gravação.
- Relação entre automação, qualidade e manutenção.

---

# O que é Automação de Testes?

Automação de testes é o uso de ferramentas, scripts e códigos para executar testes de forma automática, reduzindo a necessidade de execução manual repetitiva.

Ela permite que determinados cenários sejam executados várias vezes sempre que necessário, ajudando a equipe a validar funcionalidades de forma mais rápida e consistente.

## Ideia principal

A automação não substitui completamente o trabalho do QA manual.

Ela serve para apoiar o processo de qualidade, principalmente em testes repetitivos, regressivos e de alta frequência.

---

# Por que automatizar testes?

A automação de testes exige um esforço inicial maior na criação dos scripts, mas reduz drasticamente o tempo de execução dos testes.

Além disso, ela diminui falhas humanas na execução de testes repetitivos e permite que uma equipe menor consiga rodar os mesmos testes quantas vezes forem necessárias.

## Benefícios da automação

Alguns dos principais benefícios estudados foram:

- Agilidade.
- Eficiência.
- Redução de custos no longo prazo.
- Reutilização de cenários.
- Melhor cobertura de testes.
- Detecção precoce de falhas.
- Redução de falhas humanas.
- Execução repetida de testes com maior consistência.

---

# Agilidade

A automação garante feedback e resultados mais rápidos.

Isso ajuda a reduzir o tempo de entrega, pois a equipe consegue identificar problemas com mais velocidade durante o desenvolvimento.

## Exemplo prático

Imagine que uma equipe precisa validar o fluxo de login, cadastro, compra e pagamento a cada nova alteração no sistema.

Se esses testes forem feitos manualmente todas as vezes, o processo pode se tornar demorado.

Com a automação, esses fluxos podem ser executados rapidamente sempre que houver uma nova versão.

---

# Eficiência e custo

A automação proporciona custos mais baixos no longo prazo, pois os cenários automatizados podem ser reutilizados diversas vezes.

Apesar de existir um custo inicial para criar e manter os testes, a economia aparece com o tempo, especialmente em projetos que precisam de muitas execuções de testes regressivos.

## Exemplo prático

Um teste manual que leva 20 minutos para ser executado pode precisar ser repetido várias vezes durante uma sprint.

Ao automatizar esse teste, a equipe investe tempo na criação do script, mas depois consegue executá-lo de forma muito mais rápida e frequente.

---

# Qualidade

A automação contribui para uma melhor cobertura de testes e para a detecção precoce de falhas no sistema.

Ela também ajuda a garantir que funcionalidades importantes continuem funcionando após novas alterações.

## Relação com testes de regressão

A automação é muito útil em testes de regressão, pois permite verificar se mudanças recentes não quebraram funcionalidades que já funcionavam anteriormente.

Exemplos de fluxos que podem ser bons candidatos para automação:

- Login.
- Cadastro.
- Recuperação de senha.
- Busca.
- Carrinho de compras.
- Pagamento.
- Validações críticas de regras de negócio.

---

# O que automatizar?

Nem tudo precisa ser automatizado.

A automação deve ser aplicada com estratégia, priorizando cenários que realmente tragam valor para o projeto.

## Bons candidatos para automação

Geralmente, bons candidatos para automação são testes que:

- São executados com frequência.
- São repetitivos.
- Possuem regras claras.
- Têm resultado esperado bem definido.
- Fazem parte de fluxos críticos.
- São importantes para regressão.
- Demandam muito tempo quando feitos manualmente.

## Exemplos

| Cenário | Vale automatizar? | Motivo |
|---|---|---|
| Login com dados válidos | Sim | Fluxo crítico e repetitivo |
| Cadastro de usuário | Sim | Funcionalidade comum e importante |
| Pagamento | Sim | Alto risco para o negócio |
| Teste visual subjetivo | Nem sempre | Pode depender de análise humana |
| Exploração livre do sistema | Não totalmente | Melhor como teste exploratório manual |

---

# Cuidados na automação de testes

Durante o estudo, também compreendi que existem alguns pontos que devem ser evitados na automação.

Automatizar sem estratégia pode gerar retrabalho, manutenção excessiva e testes que não agregam valor real ao projeto.

## Pontos a serem evitados

- Automatizar sem foco.
- Criar testes inúteis.
- Criar testes sem objetivo claro.
- Automatizar cenários que ninguém vai acompanhar.
- Criar mais testes automatizados do que o time consegue manter.
- Criar automação, mas continuar rodando tudo manualmente.
- Depender demais de ferramentas de gravação.

---

# Automatizar sem foco

Automatizar sem foco significa criar testes apenas por criar, sem entender se aquele cenário realmente agrega valor ao projeto.

A automação precisa estar alinhada aos riscos, aos fluxos críticos e às necessidades do time.

## Exemplo

Automatizar uma tela pouco usada, que muda o tempo todo e não tem impacto relevante para o negócio, pode gerar mais custo de manutenção do que benefício.

---

# Sobrecarga de testes automatizados

Criar muitos testes automatizados pode parecer uma boa ideia, mas pode se tornar um problema se o time não conseguir manter esses testes.

Testes automatizados precisam ser atualizados sempre que o sistema muda.

Se a equipe não consegue acompanhar essa manutenção, a suíte de testes pode se tornar instável e pouco confiável.

## Problemas comuns

- Testes quebrando com frequência.
- Alto custo de manutenção.
- Falsos positivos.
- Falsos negativos.
- Perda de confiança nos testes.
- Tempo excessivo para corrigir scripts.

---

# Execução manual após automatizar

Outro ponto importante é evitar criar automação e, ainda assim, continuar executando os mesmos testes manualmente sem necessidade.

Se um teste foi automatizado e está confiável, ele deve reduzir o esforço manual da equipe.

Isso não significa abandonar os testes manuais, mas sim usar cada abordagem no momento certo.

---

# Ferramentas de gravação

Ferramentas de gravação, também conhecidas como Record & Play, permitem gravar ações realizadas pelo usuário e transformá-las em testes automatizados.

Um exemplo citado nas anotações foi o Selenium IDE.

## Cuidados com Record & Play

Apesar de parecerem práticas para iniciantes, essas ferramentas podem quebrar facilmente quando o sistema muda.

Isso acontece porque elas costumam depender muito da interface e da forma como os elementos aparecem na tela.

## Exemplo

Se um botão mudar de lugar, nome ou estrutura no HTML, o teste gravado pode deixar de funcionar.

Por isso, ferramentas de gravação podem ser úteis para aprendizado, mas não devem ser a única base de uma estratégia profissional de automação.

---

# Automação não substitui o raciocínio de QA

Automação de testes não é apenas escrever scripts.

Antes de automatizar, é necessário entender:

- O que testar.
- Por que testar.
- Qual risco será reduzido.
- Qual cenário tem valor.
- Qual resultado é esperado.
- Como manter o teste no futuro.
- Quando o teste deve ser executado.

Um teste mal planejado continua sendo ruim, mesmo que esteja automatizado.

---

# Testes manuais x Testes automatizados

| Critério | Teste Manual | Teste Automatizado |
|---|---|---|
| Execução | Feita por uma pessoa | Feita por ferramenta/script |
| Melhor uso | Exploração, análise crítica e cenários subjetivos | Repetição, regressão e fluxos críticos |
| Custo inicial | Menor | Maior |
| Custo no longo prazo | Pode aumentar com repetições | Pode reduzir com reutilização |
| Velocidade | Menor em testes repetitivos | Maior em execuções repetidas |
| Manutenção | Documentação e execução | Scripts e dados de teste |
| Depende de raciocínio humano? | Sim | Sim, principalmente no planejamento |

---

# Minha percepção

Neste módulo, compreendi que automação de testes é uma ferramenta poderosa, mas precisa ser usada com estratégia.

Automatizar tudo não é o objetivo.

O mais importante é automatizar os testes certos, principalmente aqueles que são repetitivos, críticos e importantes para regressão.

Também entendi que a automação não elimina a importância do QA manual. Pelo contrário, ela libera tempo para que o QA possa focar em atividades mais analíticas, como testes exploratórios, análise de riscos, melhoria dos cenários e compreensão das regras de negócio.

---

# Conclusão

Estudar automação de testes me ajudou a entender que qualidade de software depende de equilíbrio entre testes manuais e automatizados.

A automação traz agilidade, eficiência e melhor cobertura, mas exige planejamento, manutenção e foco em valor.

Um bom profissional de QA precisa saber quando automatizar, o que automatizar e quando o teste manual ainda é a melhor opção.

Este capítulo encerra o curso de Fundamentos de Teste de Software, consolidando uma base importante para os próximos estudos em QA, testes manuais, API, banco de dados, Git/GitHub, CI/CD e automação.

## Evidência de estudo

![Anotações sobre automação de testes](../images/automacao.jpeg)

## Status

Concluído.
