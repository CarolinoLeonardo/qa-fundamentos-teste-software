**# 03 - O que é Teste de Software

Esta pasta documenta meus estudos sobre os conceitos fundamentais de Teste de Software.

Nesta etapa, estudei o que é teste de software, por que testar, os princípios do teste e o custo da falta de testes.

## Assuntos estudados

- O que é Teste de Software
- Diferença entre teste e depuração
- Por que testar
- Os 7 princípios do teste
- Custo da falta de testes

---

# O que é Teste de Software?

De acordo com Bill Hetzel, teste é uma atividade direcionada para avaliar um atributo ou capacidade de um programa ou sistema e determinar se ele satisfaz os resultados requeridos.

Com base nos meus estudos, o teste de software serve para verificar se um sistema está em conformidade com as especificações, além de ajudar a descobrir defeitos ocultos.

O teste também contribui para certificar que funções indesejadas não ocorram, trazendo mais confiança sobre o desempenho do sistema e ajudando a entender os riscos envolvidos na liberação de um produto.

## Teste não é garantia absoluta

Um ponto importante estudado foi que não se pode inserir qualidade em um produto de software mal construído apenas com testes.

Ao mesmo tempo, também não é possível construir um produto de qualidade sem testes.

Ou seja, o teste é uma parte essencial da qualidade, mas ele precisa estar acompanhado de boas práticas de desenvolvimento, planejamento, análise e design.

---

# Teste x Depuração

Teste e depuração não são a mesma coisa.

Embora testadores e desenvolvedores possam se cruzar em alguns contextos, especialmente em abordagens ágeis, existe uma diferença clara entre os conceitos.

## Teste

Teste é a execução do software com o objetivo de mostrar falhas causadas por defeitos no sistema.

Em outras palavras, o teste busca identificar comportamentos incorretos, inesperados ou divergentes dos requisitos.

## Depuração

Depuração é uma atividade de desenvolvimento focada em localizar, analisar e corrigir os defeitos no código.

Enquanto o teste encontra evidências de falhas, a depuração busca a causa do problema e realiza a correção.

---

# Por que testar?

O teste de software é considerado indispensável porque atua diretamente na redução de riscos de falha e na detecção precoce de problemas.

Testar ajuda a elevar a qualidade do sistema por meio da identificação e correção de defeitos.

Além disso, a prática de teste melhora a manutenibilidade do código, ajuda a assegurar o cumprimento de requisitos contratuais e normas legais do setor, e contribui para o sucesso da entrega do produto final.

## Benefícios do teste de software

- Reduz riscos de falha.
- Identifica problemas antes da entrega ao usuário.
- Aumenta a qualidade do sistema.
- Ajuda a validar requisitos.
- Gera mais confiança na liberação do produto.
- Reduz custos de correção quando aplicado cedo.
- Melhora a experiência do usuário.
- Apoia a tomada de decisão sobre uma entrega.

---

# Os 7 princípios do teste

## 1. O teste demonstra a presença de defeitos

O teste reduz as chances de bugs permanecerem no sistema, mas não garante que ele esteja totalmente livre de defeitos.

Mesmo após muitos testes, ainda pode existir algum problema não identificado.

## 2. Teste exaustivo é impossível

Testar todas as combinações possíveis de entradas, fluxos, dados, dispositivos, navegadores e cenários é praticamente impossível.

Por isso, é necessário verificar riscos e prioridades para concentrar os esforços de teste nas principais expectativas e necessidades do sistema.

A ideia não é testar “tudo”, mas testar de forma estratégica.

## 3. Teste antecipado

O teste deve começar no início do desenvolvimento, com atividades de planejamento, análise e modelagem contendo objetivos bem definidos.

Quanto mais cedo um defeito é identificado, menor tende a ser o custo de correção.

## 4. Agrupamento de defeitos

Um número pequeno de módulos costuma concentrar a maior parte dos defeitos encontrados.

Esse princípio se relaciona com a ideia de que aproximadamente 20% dos módulos podem conter cerca de 80% dos defeitos descobertos.

Na prática, isso ajuda o QA a priorizar áreas mais críticas do sistema.

## 5. Paradoxo do Pesticida

Após determinado tempo, os mesmos testes deixam de encontrar novos erros.

Por isso, os testes precisam ser revisados, atualizados e expandidos para cobrir novos pontos do sistema e encontrar novos tipos de defeitos.

## 6. Teste depende do contexto

Cada contexto exige uma abordagem de teste diferente.

Não podemos aplicar exatamente os mesmos testes em um sistema de segurança, em um e-commerce, em um aplicativo bancário ou em uma rede social.

O tipo de produto, o risco envolvido, os usuários e os requisitos influenciam diretamente a estratégia de teste.

## 7. A ilusão da ausência de erros

Encontrar e corrigir defeitos não garante que o sistema construído atenda às expectativas e necessidades do usuário.

Um software pode estar tecnicamente correto, mas ainda assim não resolver o problema real do cliente.

Por isso, testar também envolve entender valor de negócio, usabilidade e aderência aos requisitos.

---

# Custo da falta de testes

Uma ideia importante estudada foi a relação entre tempo e dinheiro.

Quanto mais tarde um defeito é descoberto, maior tende a ser o custo para corrigi-lo.

Se um desenvolvedor ou testador encontra um bug enquanto o software ainda está sendo desenhado ou programado, a correção pode levar poucos minutos e custar pouco.

Porém, se o bug é descoberto depois que o sistema já foi entregue, o custo pode aumentar muito.

Nesse caso, pode ser necessário:

- Parar a equipe.
- Refazer código.
- Testar tudo novamente.
- Atualizar versões.
- Lidar com insatisfação do cliente.
- Corrigir problemas em produção.
- Recuperar confiança dos usuários.

## Regra 10 de Myers

A Regra 10 de Myers mostra que o custo para corrigir um bug aumenta 10 vezes a cada fase que ele avança no desenvolvimento.

Exemplo estudado:

| Fase em que o erro é encontrado | Custo relativo |
|---|---|
| Requisitos | 1 |
| Design | 10 |
| Código | 100 |
| Testes | 1.000 |
| Produção | 10.000 |

Essa regra reforça que adiar os testes pode custar exponencialmente mais caro.

---

# Exemplo prático

Imagine um sistema de compras online.

Se um erro no cálculo do frete for encontrado durante a fase de requisitos, a equipe pode corrigir a regra antes mesmo de começar o desenvolvimento.

Se esse erro for descoberto apenas em produção, a empresa poderá ter prejuízo financeiro, reclamações de clientes, retrabalho técnico e danos à reputação.

Por isso, testar cedo é uma prática essencial.

---

# Conclusão

Nesta etapa, compreendi que o teste de software é uma atividade essencial para reduzir riscos, identificar defeitos, validar requisitos e aumentar a confiança na entrega.

Também entendi que testar não significa provar que um sistema está perfeito. O teste ajuda a revelar problemas e apoiar decisões, mas a qualidade precisa ser construída desde o início do processo de desenvolvimento.

## Evidências de estudo

![Anotações sobre O que é Teste de Software](../images/02.jpeg)

![Anotações sobre Por que Testar e Princípios do Teste](../images/03.jpeg)

![Anotações sobre os 7 Princípios do Teste](../images/04.jpeg)

![Anotações sobre Custo da Falta de Testes](../images/05.jpeg)

## Status

Concluído.**
