# Diagrama de Implantação

## Introdução

No contexto da Linguagem de Modelagem Unificada (UML), o diagrama de implantação é classificado como um diagrama estrutural, responsável por representar a implementação física dos artefatos de software nos componentes de hardware do sistema. Esses artefatos correspondem aos elementos gerados durante o desenvolvimento, como serviços, aplicações e bibliotecas, enquanto os nódulos, representados por caixas tridimensionais, indicam os ambientes de execução, sejam eles dispositivos físicos ou plataformas de software <a href="#/Modelagem/2.1.ModelagemEstatica/Diagrama_de_implantacao?id=referencias-bibliograficas-1">[1]</a>.

Além disso, esse tipo de diagrama permite compreender como os elementos do sistema estão distribuídos em tempo de execução, evidenciando a topologia da infraestrutura, as conexões entre os nódulos e a forma como o software interage com o hardware <a href="#/Modelagem/2.1.ModelagemEstatica/Diagrama_de_implantacao?id=referencias-bibliograficas-2">[2]</a>. Dessa forma, torna-se uma ferramenta essencial para visualizar a arquitetura de implantação, considerando também aspectos como protocolos de comunicação, middleware e restrições do ambiente físico <a href="#/Modelagem/2.1.ModelagemEstatica/Diagrama_de_implantacao?id=referencias-bibliograficas-3">[3]</a>.

No contexto do projeto **Carona Amiga FCTE**, o diagrama de implantação desempenha um papel fundamental ao possibilitar a representação clara de como a aplicação será distribuída fisicamente, incluindo servidores, banco de dados, dispositivos dos usuários (motoristas e passageiros) e os meios de comunicação entre esses elementos. Assim, ele contribui para uma melhor compreensão da infraestrutura necessária para o funcionamento do sistema, bem como para o planejamento da sua implementação.

---

## Objetivos

Com base na elaboração do diagrama de implantação para o projeto **Carona Amiga FCTE**, têm-se como objetivos:

- Representar a arquitetura física de execução do sistema, evidenciando a relação entre software e hardware.

- Identificar e descrever os nódulos do sistema, incluindo servidores, dispositivos dos usuários e ambientes de execução.

- Demonstrar a distribuição dos artefatos de software nos diferentes nódulos.

- Evidenciar os canais de comunicação e as interações entre os componentes do sistema.

- Proporcionar uma visão clara da topologia da infraestrutura, auxiliando na compreensão do funcionamento em tempo de execução.

- Apoiar o planejamento da implementação, considerando aspectos como arquitetura de distribuição, limitações de hardware e integração entre sistemas.

---

## Metodologia

A elaboração do diagrama de implantação do projeto **Carona Amiga FCTE** foi conduzida por meio de uma abordagem analítico-descritiva, fundamentada nos artefatos de modelagem previamente produzidos pela equipe e nos requisitos elicitados ao longo da etapa de investigação do problema. Tal procedimento teve como propósito assegurar a coerência entre a arquitetura lógica do sistema e sua representação física, evidenciando os ambientes de execução, os artefatos implantados e os meios de comunicação necessários ao funcionamento da aplicação. Além dos modelos estruturais, foram considerados os requisitos identificados no artefato de [Perfil de Usuário](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario), de modo a estabelecer a rastreabilidade entre as necessidades dos usuários e os elementos contemplados na infraestrutura de implantação.

1. Em um primeiro momento, realizou-se a análise sistemática dos artefatos-base do projeto, com destaque para o [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md), o [Diagrama de Componentes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_componentes.md) e o artefato de [Perfil de Usuário](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario). Essa etapa permitiu identificar os principais elementos estruturais do sistema, suas responsabilidades, dependências, interações e requisitos associados ao contexto de uso da aplicação, fornecendo subsídios para a definição da arquitetura de implantação.

2. A partir desse levantamento, elaborou-se uma tabela de apoio com a finalidade de organizar os nós de implantação e seus respectivos papéis na infraestrutura do sistema. Nessa sistematização, foram considerados elementos como dispositivos dos usuários, aplicação e banco de dados, de modo a explicitar a distribuição dos recursos computacionais necessários e registrar a rastreabilidade entre os nós definidos e os requisitos elicitados no artefato de Perfil de Usuário.

3. Na etapa seguinte, foi construída a versão inicial do diagrama na ferramenta **Draw.io**, contemplando a representação dos nós físicos e lógicos, dos artefatos alocados em cada ambiente de execução e das relações de comunicação estabelecidas entre os componentes do sistema.

4. Por fim, o diagrama foi submetido a uma fase de [verificação](/Modelagem/2.6.VerificacaoDosDiagramas/2.6.1.VerificacaoDiagramaImplantacao.md), com o objetivo de avaliar sua consistência interna, sua aderência aos demais modelos produzidos no projeto e sua capacidade de representar adequadamente a infraestrutura necessária para a operacionalização do **Carona Amiga FCTE**.

---

## Tabela de Análise

A Tabela 1 tem como finalidade apoiar a análise e a identificação dos nós requeridos para a construção do Diagrama de Implantação do projeto **Carona Amiga FCTE**, considerando a infraestrutura representada no diagrama e os requisitos elicitados a partir do artefato de [Perfil de Usuário](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario), de modo a explicitar a rastreabilidade entre as necessidades identificadas e os elementos de implantação adotados. Para facilitar a navegação, os códigos apresentados na coluna "Requisitos Atendidos" foram associados às seções correspondentes do artefato de origem.

<details>
  <summary><strong>Tabela 1: Análise dos Nós de Implantação</strong></summary>

**Tabela 1**: Análise dos Nós de Implantação

| ID  | Tipo de Nó                 | Nome do Nó                                  | <<Estereótipo>> / Ícone Usado | Descrição / Responsabilidade                                                                                                                                                                                     | Artefatos / Componentes Implantados               | Ambiente de Execução / Software Chave | Comunicação Principal (Para/De, Protocolo)                              | Requisitos Atendidos                                                                                                                                                                                                                                                                                                                                 |
| --- | :------------------------- | :------------------------------------------ | :---------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------ | :------------------------------------ | :---------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01  | Dispositivo do Usuário     | `dispositivo-estudante: computador/celular` | `<<device>>`                  | Representa o ponto de acesso dos estudantes à plataforma. Nesse nó são executadas as interações de cadastro, consulta de caronas, configuração de preferências, chat e acompanhamento das informações da viagem. | `index.html`<br>`frontend.js`<br>`styles.css`     | Navegador Web                         | [Para] Firewall (HTTPS)                                                 | [RFU02][RFU], [RFM01][RFM], [RFM02][RFM], [RFS01][RFS], [RFS03][RFS], [RFS04][RFS], [RFF01][RFF], [RFF02][RFF], [RFF03][RFF], [RFF04][RFF], [RFF05][RFF], [RFF06][RFF], [RFF07][RFF], [RFA01][RFA], [RFA02][RFA], [RFP01][RFP], [RNFM01][RFM], [RNFF02][RFF]                                                                                         |
| 02  | Rede / Segurança           | `Firewall`                                  | `<<firewall>>`                | Atua como camada intermediária de proteção entre o dispositivo do estudante e o servidor de backend, controlando o tráfego de entrada e contribuindo para a segurança das comunicações estabelecidas no sistema. | -                                                 | Serviço de Firewall / Regras de Rede  | [De] Dispositivo-estudante (HTTPS)<br>[Para] Backend: Servidor (TCP/IP) | [RNFS01][RFS], [RNFS02][RFS], [RNFF01][RFF], [RNFA01][RFA]                                                                                                                                                                                                                                                                                           |
| 03  | Servidor de Aplicação      | `backend: Servidor`                         | `<<device>>`                  | Executa a lógica de negócio da aplicação, incluindo autenticação, gerenciamento de perfis, preferências de pareamento, processamento de caronas, chat, avaliações e demais serviços centrais da plataforma.      | `api_caronas.js`                                  | `Node.js Runtime`                     | [De] Firewall (TCP/IP)<br>[Para] Banco: Servidor (TCP/IP)               | [RFU01][RFU], [RFU02][RFU], [RFM01][RFM], [RFM02][RFM], [RFS01][RFS], [RFS02][RFS], [RFS03][RFS], [RFS04][RFS], [RFF01][RFF], [RFF02][RFF], [RFF03][RFF], [RFF04][RFF], [RFF05][RFF], [RFF06][RFF], [RFF07][RFF], [RFA01][RFA], [RFA02][RFA], [RFP01][RFP], [RNFS01][RFS], [RNFS02][RFS], [RNFF01][RFF], [RNFA01][RFA], [RNFA02][RFA], [RNFP01][RFP] |
| 04  | Servidor de Banco de Dados | `banco: Servidor`                           | `<<device>>`                  | Responsável pela persistência dos dados da aplicação, armazenando informações de usuários, veículos, corridas e conversas necessárias ao funcionamento dos serviços oferecidos pela plataforma.                  | `Usuario`<br>`Veiculo`<br>`Corrida`<br>`Conversa` | `PostgreSQL`                          | [De] Backend: Servidor (TCP/IP)                                         | [RFU01][RFU], [RFU02][RFU], [RFS02][RFS], [RFS03][RFS], [RFS04][RFS], [RFF01][RFF], [RFF02][RFF], [RFF04][RFF], [RFA01][RFA], [RFP01][RFP], [RNFS01][RFS], [RNFS02][RFS], [RNFA02][RFA], [RNFP01][RFP]                                                                                                                                               |

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

</details>

[RFU]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usuário-rfu
[RFM]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-à-motivação-do-usuário-rfm
[RFS]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-à-segurança-do-usuário-rfs
[RFF]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff
[RFA]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-à-aspectos-sociais-rfa
[RFP]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-à-pagamento-rfp

---

## Diagrama de Implantação

A fim de proporcionar uma melhor compreensão do diagrama, a Figura 1 apresenta a legenda dos elementos que o compõem.

<div style="text-align: center;">
Legenda do Diagrama de Implantação
<br>
<img src="../docs/assets/diagrama_implantacao/diagrama_implantacao.png" alt="Legenda do Diagrama de Implantação">
<font size="2"><p style="text-align: center;">Figura 1.</p></font>
</div>

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

---

### Apresentação do Diagrama de Implantação

<div style="text-align: center;">
Diagrama de Implantação, Versão 2

<br>
<img src="../docs/assets/diagrama_implantacao/diagrama_de_implantacao.png" alt="Diagrama de Implantação">
<font size="2"><p style="text-align: center">Figura 2.</p></font>
</div>

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

<div style="text-align: center;">
Diagrama de Implantação, Versão 2.
<br>
<img src="../docs/assets/diagrama_implantacao/diagrama_de_implantacao_v2.png" alt="Diagrama de Implantação">
<font size="2"><p style="text-align: center">Figura 3.</p></font>

Nota:  Com base no feedback da professora, foi realizado uma segunda versão do diagrama de implantação.

</div>

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

---

## Gravação da discussão do Diagrama de Implantação

A gravaçõe abaixo registram o processo de elaboração e discussão do Diagrama de Implantação do *Carona Amiga*, incluindo o alinhamento sobre a estrutura de implantação do sistema, os nós (dispositivos e ambientes de execução), os artefatos distribuídos e as relações de comunicação, além das principais decisões tomadas durante a modelagem.

### Reunião 1

A primeira reunião teve como foco a discussão teórica e o estudo dos conceitos relacionados ao diagrama de implantação. Já a segunda reunião foi dedicada à organização e estruturação do diagrama, definindo seus elementos e a forma de representação do sistema.

<iframe width="1321" height="743" src="https://www.youtube.com/embed/L7cldaCjV-4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/L7cldaCjV-4" target="_blank">Clique aqui para assistir no YouTube</a></p>

---

### Reunião 2

A gravaçõe abaixo registram o processo de elaboração e discussão do Diagrama de Implantação do *Carona Amiga*, incluindo o alinhamento sobre os nós, artefatos e relações de comunicação do sistema, bem como as decisões tomadas durante a modelagem.

<iframe width="1321" height="743" src="https://www.youtube.com/embed/D_kRKRohL50" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/D_kRKRohL50" target="_blank">Clique aqui para assistir no YouTube</a></p>

## Conclusão

A construção do Diagrama de Implantação do projeto **Carona Amiga FCTE** possibilitou consolidar, de forma estruturada, a visão da infraestrutura necessária para o funcionamento da plataforma, articulando os ambientes de execução, os artefatos implantados e os canais de comunicação indispensáveis à operacionalização do sistema. A representação dos dispositivos dos usuários, da camada de aplicação, do mecanismo intermediário de segurança e do banco de dados tornou mais evidente a maneira pela qual os elementos de software e hardware se relacionam para sustentar funcionalidades centrais da solução, tais como cadastro de usuários, gerenciamento de preferências, oferta e solicitação de caronas, troca de mensagens, acompanhamento de corridas e armazenamento persistente das informações.

Além disso, a elaboração deste artefato demonstrou a importância de integrar os modelos estruturais previamente desenvolvidos aos requisitos elicitados no decorrer do projeto, em especial aqueles derivados do artefato de Perfil de Usuário. Essa articulação ampliou a capacidade explicativa do diagrama, pois permitiu não apenas representar a distribuição física dos componentes, mas também evidenciar a rastreabilidade entre as necessidades identificadas junto aos usuários e os nós definidos para suportá-las em nível de implantação.

Sob essa perspectiva, o diagrama produzido contribui de maneira significativa para o entendimento da arquitetura do sistema e para o planejamento das etapas subsequentes de implementação, ao explicitar dependências técnicas, fluxos de comunicação e responsabilidades associadas a cada nó. Assim, o artefato reforça a coerência entre requisitos, modelagem e infraestrutura, constituindo-se como um instrumento relevante para a validação da solução proposta e para a redução de ambiguidades no desenvolvimento do **Carona Amiga FCTE**.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> LUCID SOFTWARE INC. **O que é diagrama de implementação UML**. Lucidchart, 2024. Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml. Acesso em: 19 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> CREATELY. **O Guia Fácil de Diagramas de Implantação UML**. Creately Blog, 2024. Disponível em: https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-implantacao/. Acesso em: 19 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> IBM CORPORATION. **Diagramas de implantação**. IBM Documentation, 2024. Disponível em: https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams. Acesso em: 19 abr. 2026 .

> <a id="referencias-bibliograficas-4">4.</a> UML-DIAGRAMS. **Deployment Diagrams Overview**. Disponível em: https://www.uml-diagrams.org/deployment-diagrams-overview.html. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-5">5.</a> Curso de UML - Diagrama de Implantação. Disponível em: https://www.youtube.com/watch?v=DgERD0HgggQ. Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                                        | Autor(es)                                                              | Revisor(es)                                                            | Detalhes da revisão |
| :----: | :--------: | -------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | :-----------------: |
|  1.0   | 16/04/2026 | Criação do documento                                                             | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | [Ana Victória Guedes da Costa](https://github.com/navicg)              | Revisão da estrutura inicial do artefato e conferência da proposta do diagrama. |
|  1.1   | 19/04/2026 | Adição da Introdução,objetivos e legenda do Diagrama de Implantação              | [Ana Victória Guedes da Costa](https://github.com/navicg)              | [João Vitor Santos de Oliveira](https://github.com/Jauzimm)            | Verificação da coerência textual entre contextualização teórica, objetivos e elementos visuais adicionados. |
|  1.2   | 20/04/2026 | Adição da metodologia e conclusão do Diagrama de Implantação                     | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | Análise da consistência entre método adotado, resultado apresentado e fechamento do artefato. |
|  1.3   | 23/04/2026 | Adição da legenda do Diagrama de Implantação                                     | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [João Vitor Santos de Oliveira](https://github.com/Jauzimm)            | Conferência da padronização visual da legenda e da correspondência com os símbolos do diagrama. |
|  1.4   | 23/04/2026 | Correção das figuras                                                             | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [Ana Victória Guedes da Costa](https://github.com/navicg)              | Revisão dos arquivos de imagem, legendas e posicionamento das figuras no documento. |
|  1.5   | 23/04/2026 | Adição do diagrama de implantação e da tabela de análise                         | [Ana Victória Guedes da Costa](https://github.com/navicg)              | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | Validação da relação entre os nós modelados, os artefatos alocados e a tabela de apoio analítica. |
|  1.6   | 23/04/2026 | Inclusão de links clicáveis de rastreabilidade na coluna de requisitos atendidos | [Ana Victória Guedes da Costa](https://github.com/navicg)              | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | Conferência da rastreabilidade entre requisitos e elementos de implantação, com foco na navegação do artefato. |
|  1.7   | 23/04/2026 | Correção os links das imagens                                                    | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [João Vitor Santos de Oliveira](https://github.com/Jauzimm)            | Revisão funcional dos links internos das imagens e ajuste de referências quebradas. |
|  1.8   | 23/04/2026 | Adição da V2 no diagrama de implantação                                          | [João Vitor Santos de Oliveira](https://github.com/Jauzimm)            | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | Avaliação das alterações feitas após feedback externo e conferência da nova versão do diagrama. |
|  1.9   | 23/04/2026 | Adição das gravações de discussões                                               | [Ana Victória Guedes da Costa](https://github.com/navicg)              | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | Revisão dos registros de reunião para garantir alinhamento entre discussões, decisões e versão publicada do artefato. |
