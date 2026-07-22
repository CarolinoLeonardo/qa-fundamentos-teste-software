# 10 - Tipos de Teste

Esta pasta documenta meus estudos sobre diferentes tipos de teste de software.

Nesta etapa, compreendi que existem vários tipos de teste, cada um com um objetivo específico dentro do processo de qualidade. Alguns testes validam funcionalidades, outros verificam desempenho, segurança, usabilidade, acessibilidade, regressão ou comportamento do sistema em diferentes ambientes.

## Objetivo desta etapa

O objetivo deste módulo foi conhecer os principais tipos de teste utilizados em projetos de software e entender em quais situações cada um pode ser aplicado.

Os tipos estudados foram:

- Teste de Configuração ou Instalação
- Teste de Integridade
- Teste de Segurança
- Teste Funcional
- Teste de Performance
- Teste de Usabilidade
- Teste de Acessibilidade
- Teste de Regressão
- Teste Exploratório

---

# Teste de Configuração ou Instalação

O teste de configuração, também chamado de teste de instalação, avalia o comportamento do software em diferentes ambientes de hardware e software.

Ele também valida o processo de instalação em diferentes cenários, como primeira instalação, atualização ou instalação personalizada com seleção de componentes.

## Objetivo

O objetivo do teste de configuração ou instalação é verificar se o sistema pode ser instalado, configurado e executado corretamente em ambientes diferentes.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Instalação inicial do sistema.
- Atualização de uma versão anterior.
- Instalação personalizada.
- Seleção de componentes durante a instalação.
- Compatibilidade com diferentes sistemas operacionais.
- Comportamento sob limitação de memória.
- Comportamento sob queda ou limitação de rede.
- Funcionamento em diferentes combinações de hardware e software.

## Exemplo prático

Imagine um aplicativo que pode ser instalado em diferentes versões do Windows.

O QA pode validar se o sistema instala corretamente no Windows 10 e Windows 11, se a atualização mantém os dados do usuário e se a instalação personalizada realmente instala apenas os componentes selecionados.

---

# Teste de Integridade

O teste de integridade testa a resistência do software às falhas, também conhecida como robustez.

Ele verifica se os componentes envolvidos permanecem íntegros mesmo com um alto volume de dados.

## Objetivo

O objetivo do teste de integridade é verificar se o sistema mantém seus dados e componentes consistentes mesmo diante de falhas, volume elevado ou situações inesperadas.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Se os dados permanecem íntegros após uma falha.
- Se o sistema mantém consistência após grande volume de operações.
- Se componentes importantes continuam funcionando após erros.
- Se transações são concluídas corretamente ou revertidas quando necessário.
- Se informações não são corrompidas durante o processamento.

## Exemplo prático

Imagine um sistema financeiro que registra transferências.

O teste de integridade pode verificar se, mesmo após uma queda de conexão durante uma transferência, o saldo do remetente e do destinatário continua correto e consistente.

---

# Teste de Segurança

O teste de segurança verifica se o sistema e os dados são acessados de maneira segura, apenas por autores ou usuários autorizados.

Esse tipo de teste busca identificar falhas de segurança em um software ou ambiente.

## Objetivo

O objetivo do teste de segurança é encontrar vulnerabilidades que possam permitir acessos indevidos, vazamento de dados ou uso incorreto do sistema.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Login e autenticação.
- Controle de acesso.
- Permissões de usuário.
- Proteção de dados sensíveis.
- Tentativas de acesso não autorizado.
- Sessões expiradas.
- Manipulação de URLs.
- Exposição indevida de informações.
- Segurança em APIs.

## Exemplo prático

Imagine um sistema com perfis de administrador e usuário comum.

O QA pode validar se um usuário comum não consegue acessar telas administrativas, mesmo tentando alterar a URL manualmente.

---

# Teste Funcional

O teste funcional pode ser manual, automatizado ou ambos.

Ele testa os requisitos funcionais, as funções do sistema e os casos de uso.

Esse teste verifica se a aplicação faz aquilo que deveria fazer.

## Objetivo

O objetivo do teste funcional é confirmar se as funcionalidades do sistema estão funcionando conforme os requisitos e regras de negócio.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Login.
- Cadastro.
- Busca.
- Edição de dados.
- Exclusão de registros.
- Carrinho de compras.
- Pagamento.
- Envio de formulário.
- Regras de negócio.

## Exemplo prático

Imagine um sistema de cadastro de usuários.

O QA pode testar se o usuário consegue se cadastrar com dados válidos, se campos obrigatórios são validados e se o sistema impede o cadastro com e-mail inválido.

---

# Teste de Performance

O teste de performance avalia o comportamento do sistema em relação ao desempenho.

Segundo minhas anotações, ele pode ser dividido em três partes principais:

- Teste de Carga
- Teste de Stress
- Teste de Estabilidade

## Teste de Carga

O teste de carga avalia o sistema em condições normais de uso.

Ele observa pontos como:

- Tempo de resposta.
- Número de transações por minuto.
- Quantidade de usuários simultâneos.
- Capacidade do sistema em uso esperado.

## Exemplo de teste de carga

Imagine um sistema que normalmente recebe 500 usuários simultâneos.

O teste de carga verifica se o sistema continua respondendo bem dentro desse volume esperado.

## Teste de Stress

O teste de stress avalia o sistema em condições extremas de uso.

Ele observa como o sistema se comporta quando é submetido a um grande volume de transações, usuários simultâneos ou picos excessivos de carga em curto período.

## Exemplo de teste de stress

Imagine uma loja virtual durante uma promoção.

O teste de stress pode simular milhares de usuários acessando o site ao mesmo tempo para verificar se o sistema suporta o pico ou se apresenta falhas.

## Teste de Estabilidade

O teste de estabilidade verifica se o sistema se mantém funcionando de maneira satisfatória após um determinado período de tempo.

## Exemplo de teste de estabilidade

Imagine um sistema que precisa ficar disponível 24 horas por dia.

O teste de estabilidade pode verificar se ele continua funcionando corretamente após muitas horas ou dias de uso contínuo.

---

# Teste de Usabilidade

O teste de usabilidade foca na experiência do usuário, também conhecida como UX.

Ele avalia a consistência da interface e a facilidade de navegação no ambiente real de uso, garantindo que o sistema seja prático e eficiente no dia a dia.

## Objetivo

O objetivo do teste de usabilidade é verificar se o usuário consegue utilizar o sistema com facilidade, clareza e eficiência.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Clareza dos botões.
- Organização das telas.
- Facilidade de navegação.
- Quantidade de passos para concluir uma ação.
- Mensagens compreensíveis.
- Consistência visual.
- Facilidade para encontrar informações.
- Experiência geral do usuário.

## Exemplo prático

Imagine um aplicativo de delivery.

O teste de usabilidade pode avaliar se o usuário consegue encontrar um restaurante, escolher um produto, adicionar ao carrinho e finalizar o pedido sem dificuldade.

---

# Teste de Acessibilidade

O teste de acessibilidade é um subconjunto dos testes de usabilidade.

Ele garante que o software possa ser utilizado por pessoas com diferentes habilidades e deficiências, como visuais, físicas, auditivas e cognitivas.

Para orientar testes na web e mobile, podem ser utilizadas as diretrizes da WCAG, recomendadas pelo W3C.

## Objetivo

O objetivo do teste de acessibilidade é verificar se o sistema pode ser utilizado pelo maior número possível de pessoas, incluindo pessoas com deficiência.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Navegação por teclado.
- Contraste adequado de cores.
- Textos alternativos em imagens.
- Compatibilidade com leitores de tela.
- Tamanho e legibilidade dos textos.
- Botões e campos com nomes acessíveis.
- Mensagens de erro compreensíveis.
- Estrutura correta de títulos e formulários.

## Exemplo prático

Imagine um formulário de cadastro.

O teste de acessibilidade pode verificar se todos os campos possuem rótulos compreensíveis, se o usuário consegue navegar apenas com o teclado e se leitores de tela conseguem identificar corretamente os elementos.

---

# Teste de Regressão

O teste de regressão consiste em testar a versão mais recente do software para garantir que novas alterações ou componentes não tenham quebrado funcionalidades que já funcionavam.

Quando uma funcionalidade que antes funcionava passa a apresentar erro após uma alteração, isso caracteriza uma regressão.

É muito comum utilizar testes automatizados para esse tipo de validação.

## Objetivo

O objetivo do teste de regressão é garantir que mudanças recentes não tenham causado efeitos colaterais em partes já existentes do sistema.

## Exemplos de validação

Esse tipo de teste pode verificar:

- Funcionalidades principais após uma nova versão.
- Correções de bugs.
- Impactos causados por novas funcionalidades.
- Fluxos críticos do sistema.
- Integrações que já funcionavam anteriormente.
- Comportamentos que não deveriam ter sido alterados.

## Exemplo prático

Imagine que uma equipe alterou a tela de cadastro de usuário.

Depois dessa alteração, o QA realiza testes de regressão para garantir que login, recuperação de senha, edição de perfil e permissões de usuário continuam funcionando corretamente.

---

# Teste Exploratório

O teste exploratório consiste em criar e executar testes simultaneamente, sem um roteiro prévio totalmente definido.

Sua eficácia depende da intuição e experiência do testador para explorar o sistema, formular cenários na hora e encontrar bugs ocultos.

## Objetivo

O objetivo do teste exploratório é descobrir problemas que talvez não tenham sido previstos nos casos de teste formais.

## Características

- Não segue um roteiro fixo.
- Depende da experiência do testador.
- Permite liberdade de investigação.
- Ajuda a encontrar bugs ocultos.
- Pode complementar testes documentados.
- É útil quando há pouco tempo ou pouca documentação.

## Exemplo prático

Imagine que o QA está testando uma nova tela de cadastro.

Além de seguir os casos de teste planejados, ele pode explorar comportamentos como:

- Digitar muitos caracteres.
- Usar caracteres especiais.
- Voltar e avançar páginas.
- Atualizar a tela durante o preenchimento.
- Enviar o formulário várias vezes.
- Testar campos em ordem diferente da esperada.

---

# Comparação entre os tipos de teste

| Tipo de Teste | Principal objetivo |
|---|---|
| Configuração ou Instalação | Validar instalação e comportamento em diferentes ambientes |
| Integridade | Verificar robustez e consistência dos dados |
| Segurança | Identificar falhas de acesso e proteção de dados |
| Funcional | Validar requisitos, funções e casos de uso |
| Performance | Avaliar desempenho, carga, stress e estabilidade |
| Usabilidade | Avaliar experiência e facilidade de uso |
| Acessibilidade | Garantir uso por pessoas com diferentes habilidades |
| Regressão | Verificar se novas mudanças não quebraram funcionalidades antigas |
| Exploratório | Descobrir bugs por investigação livre |

---

# Minha percepção

Neste módulo, compreendi que cada tipo de teste possui um objetivo específico dentro da qualidade de software.

O teste funcional valida se o sistema faz o que deveria fazer.

O teste de segurança protege dados e acessos.

O teste de performance avalia como o sistema se comporta sob diferentes cargas.

O teste de usabilidade e acessibilidade analisam a experiência das pessoas que utilizam o produto.

O teste de regressão protege funcionalidades já existentes após mudanças.

Já o teste exploratório permite investigar o sistema de forma mais livre, buscando problemas que talvez não tenham sido previstos nos casos de teste.

---

# Conclusão

Estudar os tipos de teste me ajudou a entender que qualidade de software envolve muito mais do que verificar se uma funcionalidade está funcionando.

Um bom processo de QA considera comportamento, segurança, desempenho, acessibilidade, usabilidade, estabilidade, integridade e riscos de mudanças.

Cada tipo de teste contribui de forma diferente para aumentar a confiança na entrega do produto final.

## Evidências de estudo

![Anotações sobre tipos de teste - Parte 1](../images/tipos1.jpeg)

![Anotações sobre tipos de teste - Parte 2](../images/tipos2.jpeg)

![Anotações sobre tipos de teste - Parte 3](../images/tipos3.jpeg)

## Status

Concluído.
