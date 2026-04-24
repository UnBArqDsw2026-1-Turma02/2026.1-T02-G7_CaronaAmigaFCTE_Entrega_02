# Verificação do Diagrama de Implantação

## Introdução

No contexto da UML, o diagrama de implantação é responsável por representar a arquitetura física de execução do sistema, evidenciando os nós, os artefatos distribuídos e os canais de comunicação entre os ambientes envolvidos. No projeto **Carona Amiga FCTE**, esse artefato foi elaborado para demonstrar a organização da infraestrutura da aplicação, contemplando o dispositivo do estudante, o firewall, o servidor de backend e o servidor de banco de dados.

A verificação desse diagrama é importante para orientar a análise da distribuição dos elementos de software e hardware, buscando coerência com a proposta da solução, com os demais artefatos de modelagem e com os requisitos considerados no projeto.

---

## Objetivos da verificação

Com base no Diagrama de Implantação do projeto **Carona Amiga FCTE**, este artefato tem como objetivos:

- Verificar se os nós representados no diagrama estão coerentes com a infraestrutura proposta para o sistema.
- Avaliar se os artefatos e componentes foram alocados de forma compatível com as responsabilidades de cada nó.
- Confirmar se os caminhos de comunicação estão consistentes com a arquitetura definida.
- Identificar se o diagrama mantém aderência aos demais artefatos de modelagem e aos requisitos levantados no projeto.

---

## Metodologia

A verificação foi conduzida a partir da análise do [Diagrama de Implantação](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_implantacao.md), de sua tabela de análise e dos artefatos utilizados como base para sua construção, especialmente o [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md), o [Diagrama de Componentes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_componentes.md) e o artefato de [Perfil de Usuário](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario).

Para isso, foram observados três aspectos principais:

1. Clareza e adequação dos nós de implantação representados na arquitetura.
2. Coerência entre artefatos, componentes implantados e responsabilidades atribuídas a cada nó.
3. Consistência dos caminhos de comunicação com a topologia proposta para o sistema.

A partir desses critérios, foi elaborada a checklist a seguir para apoiar a revisão do artefato. As tabelas abaixo funcionam como instrumento de conferência e não indicam, neste momento, a execução final da verificação.

---

## Tabelas de Verificação

<details>
  <summary><strong>Tabela 1: Verificação dos Nós de Implantação</strong></summary>

| ID  | Pergunta de Verificação | Verificado | Rastreabilidade |
| --- | :---------------------- | :--------: | :-------------- |
| 01 | Os nós do diagrama correspondem aos elementos definidos na tabela de análise (`dispositivo-estudante`, `Firewall`, `backend: Servidor` e `banco: Servidor`)? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [Edraw](https://www.edrawsoft.com/pt/deployment-chart-example.html) |
| 02 | Os nomes e estereótipos dos nós estão coerentes com seus papéis na infraestrutura do sistema? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [IBM](https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams), [UML Diagrams](https://www.uml-diagrams.org/deployment-diagrams-overview.html) |
| 03 | As responsabilidades atribuídas a cada nó estão alinhadas às funcionalidades e aos requisitos considerados no projeto? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [Edraw](https://www.edrawsoft.com/pt/deployment-chart-example.html) |
| 04 | Os ambientes de execução principais foram identificados de forma consistente (`Navegador Web`, serviço de firewall, `Node.js Runtime` e `PostgreSQL`)? | Verificado | [OMG](https://www.omg.org/spec/UML/), [IBM](https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams) |
| 05 | A arquitetura representada separa de forma clara as camadas de cliente, segurança, aplicação e persistência? | Verificado | [OMG](https://www.omg.org/spec/UML/), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-deployment-diagram/) |

</details>

<details>
  <summary><strong>Tabela 2: Verificação dos Artefatos e Caminhos de Comunicação</strong></summary>

| ID  | Pergunta de Verificação | Verificado | Rastreabilidade |
| --- | :---------------------- | :--------: | :-------------- |
| 01 | Os artefatos e componentes associados a cada nó estão coerentes com a tabela de análise do diagrama? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-deployment-diagram/) |
| 02 | A distribuição entre front-end no dispositivo do usuário, lógica de negócio no backend e persistência no banco está representada de forma clara? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [Edraw](https://www.edrawsoft.com/pt/deployment-chart-example.html) |
| 03 | Os caminhos de comunicação representam corretamente o fluxo entre dispositivo do estudante, firewall, backend e banco de dados? | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml), [Edraw](https://www.edrawsoft.com/pt/deployment-chart-example.html) |
| 04 | Os protocolos indicados nos canais de comunicação, como HTTPS e TCP/IP, estão compatíveis com a arquitetura proposta? | Verificado | [OMG](https://www.omg.org/spec/UML/), [IBM](https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams) |
| 05 | O diagrama está consistente com os diagramas de classes e componentes utilizados como base para sua elaboração? | Verificado | [UML Diagrams](https://www.uml-diagrams.org/deployment-diagrams-overview.html), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-deployment-diagram/) |

</details>

---

## Vídeo de Verificação do Diagrama

<iframe width="1321" height="743" src="https://www.youtube.com/embed/YPZcmYfgGVE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/YPZcmYfgGVE" target="_blank">Clique aqui para assistir no YouTube</a></p>

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

---

## Conclusão

O presente artefato organiza critérios para a verificação do Diagrama de Implantação do projeto **Carona Amiga FCTE**, com foco nos nós da infraestrutura, na distribuição dos artefatos e nos caminhos de comunicação entre as camadas da solução. As tabelas propostas servem como apoio para a análise da aderência do diagrama às convenções da UML e à arquitetura definida para o sistema.

Desse modo, o documento contribui para orientar a revisão do artefato e para reduzir ambiguidades na compreensão da infraestrutura representada, sem antecipar resultados de uma verificação ainda não concluída.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> EDRAWSOFT. **Exemplos de Diagrama de Implantação UML**. Edraw, 2024. Disponível em: https://www.edrawsoft.com/pt/deployment-chart-example.html. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> IBM CORPORATION. **Diagramas de implantação**. IBM Documentation, 2024. Disponível em: https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> LUCID SOFTWARE INC. **O que é diagrama de implementação UML**. Lucidchart, 2024. Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-4">4.</a> Object Management Group (OMG). **Unified Modeling Language (UML) Specification**. Version 2.5.1. 2017. Disponível em: https://www.omg.org/spec/UML/. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-5">5.</a> UML-DIAGRAMS. **Deployment Diagrams Overview**. UML Diagrams.org, 2024. Disponível em: https://www.uml-diagrams.org/deployment-diagrams-overview.html. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-6">6.</a> VISUAL PARADIGM. **What is Deployment Diagram?** Visual Paradigm Guide, 2024. Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-deployment-diagram/. Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--------: | --------- | --------- | ----------- | :-----------------: |
|  1.0   | 23/04/2026 | Elaboração do artefato de verificação alinhado ao Diagrama de Implantação | [Ana Victória Guedes da Costa](https://github.com/navicg) | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado |
|  1.1   | 23/04/2026 | Elaboração das perguntas | [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato revisado |
|  1.2   | 23/04/2026 | Adição do vídeo de verificação, e status da verificação           | [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato revisado |
