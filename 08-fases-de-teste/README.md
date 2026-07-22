# 11 - Fases de Teste

Esta pasta documenta meus estudos sobre as principais fases de teste dentro do processo de desenvolvimento de software.

Nesta etapa, compreendi que os testes podem acontecer em diferentes momentos e níveis, desde a validação de pequenas unidades do sistema até a verificação do sistema completo antes da entrega ao usuário final.

## Objetivo desta etapa

O objetivo deste módulo foi entender as principais fases de teste e como cada uma delas contribui para a qualidade do software.

As fases estudadas foram:

- Teste de Unidade
- Teste de Integração
- Teste de Sistema
- Teste de Aceitação

---

# Teste de Unidade

O teste de unidade, também chamado de teste unitário, é a fase em que cada unidade do sistema é testada individualmente.

Normalmente, é responsabilidade do desenvolvedor realizar esse tipo de teste após codificar uma parte específica do sistema.

## Objetivo

O objetivo do teste de unidade é isolar cada parte do sistema para garantir que ela esteja funcionando conforme especificado.

## Características

- Testa partes pequenas do sistema.
- Geralmente é realizado pelo desenvolvedor.
- Costuma acontecer no ambiente de desenvolvimento.
- Ajuda a identificar problemas logo após a codificação.
- Pode ser automatizado.

## Exemplo prático

Imagine uma função responsável por calcular o desconto de um produto.

Antes de testar o sistema inteiro, o desenvolvedor pode testar apenas essa função, verificando se ela retorna o valor correto para diferentes porcentagens de desconto.

---

# Teste de Integração

O teste de integração é realizado antes, durante ou após a integração de um novo módulo ao pacote principal de software.

Essa fase envolve o teste de cada módulo de código individual em conjunto com outros módulos.

## Objetivo

O objetivo do teste de integração é verificar se diferentes partes do sistema funcionam corretamente quando trabalham juntas.

## Características

- Testa a comunicação entre módulos.
- Pode envolver desenvolvedores e analistas de sistemas.
- Geralmente ocorre em ambiente de desenvolvimento.
- Ajuda a identificar problemas de comunicação entre partes do sistema.
- Pode revelar erros que não aparecem nos testes unitários.

## Exemplo prático

Imagine um sistema de e-commerce com dois módulos:

- Módulo de carrinho.
- Módulo de pagamento.

Mesmo que cada módulo funcione corretamente de forma isolada, é necessário testar se o carrinho envia corretamente as informações de valor, produtos e frete para o módulo de pagamento.

---

# Teste de Sistema

O teste de sistema garante que o sistema funcione como um todo, com todas as unidades trabalhando juntas.

Também é chamado de teste de caixa preta, pois o sistema é testado com tudo conectado, incluindo banco de dados, serviços web, jobs e demais integrações.

## Objetivo

O objetivo do teste de sistema é validar o comportamento completo do software em um ambiente mais próximo do real.

## Características

- Testa o sistema completo.
- É executado com os módulos integrados.
- Pode envolver banco de dados, APIs, serviços web e rotinas internas.
- Geralmente é realizado por analistas de teste.
- Costuma acontecer em ambiente de testes.
- Trabalha com maior volume de dados.

## Exemplo prático

Imagine um fluxo completo de compra em um e-commerce.

No teste de sistema, o QA poderia validar o seguinte fluxo:

1. Acessar o site.
2. Fazer login.
3. Escolher um produto.
4. Adicionar ao carrinho.
5. Aplicar cupom de desconto.
6. Escolher forma de pagamento.
7. Finalizar a compra.
8. Verificar se o pedido foi registrado corretamente.

Nesse caso, o teste não valida apenas uma função isolada, mas o comportamento do sistema como um todo.

---

# Teste de Aceitação

O teste de aceitação verifica a conformidade do sistema com os requisitos de negócio e as necessidades do usuário.

Ele acontece na última fase do ciclo de desenvolvimento, validando se a entrega está adequada.

Geralmente, é realizado por um grupo restrito de usuários ou representantes do negócio, em um ambiente diferente do ambiente de teste de sistema.

## Objetivo

O objetivo do teste de aceitação é confirmar se o sistema atende ao que foi solicitado pelo negócio e se está pronto para ser entregue ou utilizado.

## Características

- Valida requisitos de negócio.
- Pode envolver usuários, analistas de negócio e analistas de teste.
- Costuma usar dados reais.
- Pode ocorrer em ambiente de UAT, pré-produção ou produção controlada.
- Ajuda a decidir se o produto pode ser aceito ou liberado.

## Exemplo prático

Imagine que uma empresa solicitou uma funcionalidade para gerar relatórios financeiros mensais.

No teste de aceitação, o usuário de negócio verifica se o relatório apresenta as informações necessárias, no formato esperado e de acordo com a regra da empresa.

---

# Comparação entre as fases de teste

| Fase | Escopo | Equipe envolvida | Dados utilizados | Ambiente |
|---|---|---|---|---|
| Teste de Unidade | Unidades isoladas | Desenvolvedores | Criados de forma automática ou manual | Desenvolvimento |
| Teste de Integração | Conjunto de unidades agrupadas | Desenvolvedores e analistas de sistemas | Criação manual | Desenvolvimento |
| Teste de Sistema | Sistema completo | Analistas de teste | Dados reais ou simulados | Testes |
| Teste de Aceitação | Sistema completo | Analistas de teste, negócio e usuários | Dados reais | UAT, pré-produção ou produção |

---

# Diferença entre as fases

## Teste de Unidade

Verifica se uma pequena parte do sistema funciona corretamente de forma isolada.

## Teste de Integração

Verifica se diferentes partes do sistema funcionam corretamente juntas.

## Teste de Sistema

Verifica se o sistema completo funciona corretamente com todos os componentes conectados.

## Teste de Aceitação

Verifica se o sistema atende às necessidades do negócio e dos usuários finais.

---

# Minha percepção

Nesta etapa, entendi que cada fase de teste tem um objetivo diferente.

O teste de unidade ajuda a validar pequenas partes do código.

O teste de integração verifica se os módulos se comunicam corretamente.

O teste de sistema valida o funcionamento completo da aplicação.

Já o teste de aceitação confirma se o produto realmente atende às necessidades do negócio e dos usuários.

Também percebi que, quanto mais avançada a fase de teste, maior tende a ser o impacto de uma falha encontrada, pois o sistema está mais próximo da entrega final.

---

# Conclusão

Estudar as fases de teste me ajudou a entender que a qualidade do software deve ser construída e validada em diferentes níveis.

Cada fase contribui para reduzir riscos, encontrar defeitos e aumentar a confiança na entrega.

Um bom processo de QA não depende apenas de testar o sistema no final, mas de validar o software desde as menores unidades até o produto completo em condições próximas da realidade.

## Evidências de estudo

![Anotações sobre fases de teste - Parte 1](../images/fasesteste1.jpeg)

![Anotações sobre fases de teste - Parte 2](../images/fasesteste2.jpeg)

## Status

Concluído.
