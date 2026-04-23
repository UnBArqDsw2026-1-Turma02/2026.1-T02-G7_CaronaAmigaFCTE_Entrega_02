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

A elaboração do diagrama de implantação do projeto **Carona Amiga FCTE** foi realizada com base nos artefatos já produzidos pela equipe, buscando representar de forma clara a estrutura física do sistema.

1. Inicialmente será realizada uma análise do material base a partir de:

- [Projeto](/Projeto/Projeto.md);
- [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md);
- [Diagrama de Componentes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_componentes.md).

2. Com base nessa análise, será elaborada uma tabela de apoio para organizar os nós de implantação necessários ao sistema, como dispositivos dos usuários, aplicação e banco de dados.

3. Em seguida, será construída a versão inicial do diagrama na ferramenta **Miro**, com a identificação dos nós, artefatos e relações de comunicação entre os elementos.

4. Após a construção, o diagrama passará por uma fase de [verificação](/Modelagem/2.6.VerificacaoDosDiagramas/2.6.1.VerificacaoDiagramaImplantacao.md), com o objetivo de garantir sua coerência.

---

## Tabela de Análise

---

## Diagrama de Implantação

<div style="text-align: center;">
Legenda do Diagrama de Implantação  
<br>
<img src="https://i.postimg.cc/8khN5Bqk/image.png" alt="figura 1">
<font size="2"><p style="text-align: center">Figura 01.</p></font>
</div>

<!-- | Elemento                         | Representação | Descrição                                                                                                                                                                       |
| -------------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Nó (Node)**                    |               | Entidade física ou virtual responsável por executar componentes do sistema. Pode representar dispositivos de hardware (como servidores e smartphones) ou ambientes de software. |
| **Dispositivo**                  |               | Representa um recurso computacional físico dentro do sistema, como servidores, máquinas cliente ou dispositivos móveis.                                                         |
| **Componente**                   |               | Unidade lógica do sistema que encapsula funcionalidades específicas e que é implantada dentro de um nó.                                                                         |
| **Artefato**                     |               | Elemento concreto gerado durante o desenvolvimento, como arquivos executáveis, bibliotecas, scripts ou arquivos de configuração.                                                |
| **Especificação de Implantação** |               | Define configurações necessárias para a implantação de um artefato em um nó, como parâmetros, scripts ou arquivos XML.                                                          |
| **Caminho de Comunicação**       |               | Representa a conexão entre dois nós, indicando o canal e, possivelmente, o protocolo de comunicação utilizado.                                                                  |
| **Pacote**                       |               | Utilizado para agrupar elementos do diagrama, organizando nós, artefatos e componentes dentro de uma mesma estrutura lógica.                                                    | -->

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

---

## Conclusão

A construção do Diagrama de Implantação do projeto **Carona Amiga FCTE** possibilitou consolidar, em uma visão única, a infraestrutura necessária para o funcionamento da plataforma de compartilhamento de caronas entre estudantes e colaboradores da FCTE. A representação dos dispositivos dos usuários, da aplicação e do banco de dados tornou mais clara a forma como os elementos do sistema se distribuem fisicamente para viabilizar funcionalidades como oferta e solicitação de caronas, comunicação entre motorista e passageiro e armazenamento das informações.

Dessa forma, o artefato contribui para o entendimento da arquitetura do sistema e apoia o planejamento das próximas etapas do projeto, ao evidenciar os ambientes de execução, os fluxos de comunicação e as dependências técnicas envolvidas na solução. Assim, o diagrama reforça a coerência entre os requisitos levantados, os modelos já produzidos pela equipe e a futura implementação do **Carona Amiga FCTE**.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> LUCID SOFTWARE INC. **O que é diagrama de implementação UML**. Lucidchart, 2024. Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml. Acesso em: 19 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> CREATELY. **O Guia Fácil de Diagramas de Implantação UML**. Creately Blog, 2024. Disponível em: https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-implantacao/. Acesso em: 19 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> IBM CORPORATION. **Diagramas de implantação**. IBM Documentation, 2024. Disponível em: https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams. Acesso em: 19 abr. 2026 .

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                           | Autor(es)                                                              | Revisor(es)                                                            | Detalhes da revisão |
| :----: | :--------: | ------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | :-----------------: |
|  1.0   | 16/04/2026 | Criação do documento                                                | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | [Ana Victória Guedes da Costa](https://github.com/navicg)              |  Artefato revisado  |
|  1.1   | 19/04/2026 | Adição da Introdução,objetivos e legenda do Diagrama de Implantação | [Ana Victória Guedes da Costa](https://github.com/navicg)              | [João Vitor Santos de Oliveira](https://github.com/Jauzimm)            |  Artefato revisado  |
|  1.2   | 20/04/2026 | Adição da metodologia e conclusão do Diagrama de Implantação        | [Karoline Luz da Conceição](https://github.com/KarolineLuz)            | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | Artefato atualizado |
|  1.3   | 23/04/2026 | Adição da legenda do Diagrama de Implantação                        | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) |                                                                        |                     |
