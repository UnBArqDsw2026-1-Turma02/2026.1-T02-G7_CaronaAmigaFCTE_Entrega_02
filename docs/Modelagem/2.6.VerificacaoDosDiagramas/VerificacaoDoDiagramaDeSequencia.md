# Verificação do Diagrama de Sequência

## Introdução

No contexto da UML, o diagrama de sequência é utilizado para representar o comportamento dinâmico do sistema, evidenciando a troca de mensagens entre atores, objetos e componentes ao longo do tempo. No projeto **Carona Amiga FCTE**, esse artefato foi elaborado para detalhar fluxos centrais da aplicação, como cadastro, login, busca de caronas, solicitação de participação, publicação de carona e confirmação de embarque.

A verificação desses diagramas é importante para orientar a análise da ordem temporal das interações, da clareza das mensagens e da coerência entre o comportamento modelado, os requisitos do sistema e os demais artefatos produzidos no projeto.

---

## Objetivos da verificação

Com base nos Diagramas de Sequência do projeto **Carona Amiga FCTE**, este artefato tem como objetivos:

- Verificar se os participantes e as linhas de vida estão representados de forma coerente com os cenários modelados.
- Avaliar se as mensagens e retornos respeitam a ordem temporal das interações descritas nos fluxos.
- Confirmar se os diagramas mantêm aderência à notação UML adotada pela equipe.
- Identificar se os diagramas estão consistentes com os requisitos e com os demais artefatos de modelagem do projeto.

---

## Metodologia

A elaboração deste artefato considerou como base o [Diagrama de Sequência](/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia.md), os fluxos descritos para o **Carona Amiga FCTE**, o protótipo de alta fidelidade do projeto e os diagramas estruturais já desenvolvidos, especialmente o [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md) e o [Diagrama de Componentes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_componentes.md).

Para a construção da checklist, foram observados três aspectos principais:

1. Clareza na identificação dos participantes, atores, objetos e linhas de vida.
2. Coerência das mensagens trocadas entre os elementos ao longo da sequência temporal.
3. Consistência entre os fluxos representados, os requisitos priorizados e a notação UML utilizada.

As tabelas abaixo funcionam como instrumento de conferência e não indicam, neste momento, a execução final da verificação.

---

## Tabelas de Verificação

<details>
  <summary><strong>Tabela 1: Verificação de Lifelines, Atores e Objetos</strong></summary>

| ID  | Pergunta de Verificação | Verificado | Rastreabilidade |
| --- | :---------------------- | :--------: | :-------------- |
| 01 | As lifelines estão representadas de forma clara, identificando corretamente atores, interfaces, serviços e banco de dados nos fluxos modelados? |  | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml), [UML Diagrams](https://www.uml-diagrams.org/sequence-diagrams.html) |
| 02 | Os participantes possuem nomes coerentes com seus papéis no sistema, como `Usuário`, `Passageiro`, `Motorista`, `:App Passageiro`, `:Ride API` e `:Banco de Dados`? |  | [IBM](https://www.ibm.com/docs/pt-br/rational-soft-arch/9.7.0?topic=diagrams-sequence), [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml) |
| 03 | A disposição dos participantes favorece a leitura da interação, mantendo atores e componentes organizados de forma lógica ao longo do fluxo? |  | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml), [Creately](https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-sequencia/) |
| 04 | As barras de ativação e demais elementos visuais de processamento estão sendo usadas de forma coerente quando necessárias? |  | [UML Diagrams](https://www.uml-diagrams.org/sequence-diagrams.html), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-sequence-diagram-tutorial/) |
| 05 | Os participantes representados nos diagramas estão consistentes com os elementos descritos nas tabelas de análise de cada fluxo? |  | Apostila UML, [Protótipo de Alta Fidelidade](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo) |

</details>

<details>
  <summary><strong>Tabela 2: Verificação de Mensagens e Fragmentos de Interação</strong></summary>

| ID  | Pergunta de Verificação | Verificado | Rastreabilidade |
| --- | :---------------------- | :--------: | :-------------- |
| 01 | As mensagens estão nomeadas de forma clara e compatível com as operações esperadas em cada fluxo, como `enviarCredenciais()`, `buscarCaronas()` e `confirmarEmbarque()`? |  | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml), [IBM](https://www.ibm.com/docs/pt-br/rational-soft-arch/9.7.0?topic=diagrams-sequence) |
| 02 | A ordem das mensagens, de cima para baixo, representa corretamente a sequência temporal das interações modeladas? |  | [UML Diagrams](https://www.uml-diagrams.org/sequence-diagrams.html), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-sequence-diagram-tutorial/) |
| 03 | Os retornos e respostas estão representados de forma coerente com o comportamento esperado dos cenários de cadastro, login, busca e confirmação? |  | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml), [UML Diagrams](https://www.uml-diagrams.org/sequence-diagrams.html) |
| 04 | Os fluxos alternativos ou condicionais, quando necessários, estão indicados de maneira adequada para representar erro, sucesso ou ausência de resultados? |  | [IBM](https://www.ibm.com/docs/pt-br/rational-soft-arch/9.7.0?topic=diagrams-sequence), [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-sequence-diagram-tutorial/) |
| 05 | As mensagens apresentadas nos diagramas estão coerentes com os requisitos e com os fluxos descritos no artefato principal de sequência? |  | Apostila UML, [Protótipo de Alta Fidelidade](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo), [Creately](https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-sequencia/) |

</details>

---
## Vídeo de Verificação do Diagrama

<iframe width="1321" height="743" src="https://www.youtube.com/embed/lEFFf72zMhw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/lEFFf72zMhw" target="_blank">Clique aqui para assistir no YouTube</a></p>

<font size="2"><p style="text-align: center">Fonte: [Ana Victória Guedes da Costa](https://github.com/navicg) e [Karoline Luz da Conceição](https://github.com/KarolineLuz), 2026.</p></font>

---

## Conclusão

O presente artefato organiza critérios para a verificação dos Diagramas de Sequência do projeto **Carona Amiga FCTE**, com foco na identificação dos participantes, na ordem das mensagens e na coerência entre os fluxos modelados e a notação UML. As tabelas propostas servem como apoio para a análise dos cenários descritos no documento principal.

Desse modo, o documento contribui para orientar a revisão dos diagramas e para reduzir ambiguidades na compreensão do comportamento dinâmico do sistema, sem antecipar resultados de uma verificação ainda não concluída.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> APOSTILA UML. **Unified Modeling Language – Linguagem de Modelagem Unificada em Português**. Seção sobre diagrama de sequência. Disponibilizada pela professora. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> CARONA AMIGA FCTE. **Protótipo de Alta Fidelidade**. Disponível em: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> CREATELY. **Tutorial do Diagrama de Sequência: Guia completo com exemplos**. Disponível em: https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-sequencia/. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-4">4.</a> IBM. **Diagramas de Sequência**. Rational Software Architect. Disponível em: https://www.ibm.com/docs/pt-br/rational-soft-arch/9.7.0?topic=diagrams-sequence. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-5">5.</a> LUCIDCHART. **O que é um diagrama de sequência UML?** Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-6">6.</a> UML DIAGRAMS. **UML Sequence Diagrams Overview**. Disponível em: https://www.uml-diagrams.org/sequence-diagrams.html. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-7">7.</a> VISUAL PARADIGM. **UML Sequence Diagram Tutorial (What is Sequence Diagram?)**. Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-sequence-diagram-tutorial/. Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão | Data       | Descrição | Autor(es) | Revisor(es) | Detalhes da Revisão |
| ------ | ---------- | --------- | --------- | ----------- | ------------------- |
| 1.0    | 23/04/2026 | Elaboração do artefato de verificação alinhado ao Diagrama de Sequência | [Ana Victória Guedes da Costa](https://github.com/navicg) | [João Vitor Santos de Oliveira](https://github.com/Jauzimm) | Artefato revisado |
|  1.1   | 23/04/2026 | Elaboração das perguntas | [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Luiza da Silva Pugas](https://github.com/Luizaxx) | Artefato revisado |
