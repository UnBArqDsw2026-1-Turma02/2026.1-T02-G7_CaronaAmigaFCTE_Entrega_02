# Verificação do Diagrama de Estados

## Introdução

O Diagrama de Estados, conforme definido pela UML, é utilizado para representar o comportamento dinâmico de um elemento do sistema ao longo do tempo, evidenciando seus estados possíveis e as transições que ocorrem em resposta a eventos, condições de guarda e ações.

No projeto **Carona Amiga FCTE**, o Diagrama de Estados foi elaborado para modelar o ciclo de vida do sistema, representando sua evolução desde a publicação até sua conclusão ou cancelamento.

A verificação desse diagrama é fundamental para garantir que os estados modelados estejam coerentes com as regras de negócio, que as transições representem corretamente os eventos do sistema e que não existam inconsistências comportamentais.

---

## Objetivo da Verificação

O objetivo da verificação do Diagrama de Estados é garantir que o modelo comportamental do sistema esteja correto, completo e consistente com os requisitos do sistema.

Busca-se:

- Verificar se os estados representam corretamente o ciclo de vida do sistema.
- Avaliar se as transições estão associadas a eventos válidos e coerentes com o domínio do problema.
- Confirmar se as condições de guarda e ações estão corretamente especificadas.
- Identificar possíveis inconsistências, estados inalcançáveis ou transições ambíguas.
- Garantir aderência às convenções da UML para Diagramas de Estados.

---

## Metodologia

A metodologia de verificação foi conduzida a partir:

- Da análise do Diagrama de Estados do ciclo de vida do sistema.
- Dos requisitos funcionais relacionados à criação, participação, início, cancelamento e conclusão de caronas.
- Da especificação UML 2.5.1 (OMG).

Foram observados quatro aspectos principais:

1. Correção da notação UML.
2. Coerência do fluxo de estados.
3. Consistência das regras de negócio.
4. Completude do ciclo de vida modelado.

---

## Tabela 1: Verificação dos Estados e Estrutura Geral

| ID  | Pergunta de Verificação                                                                                                   | Verificado | Rastreabilidade                                                                                                                                                   |
| --- | ------------------------------------------------------------------------------------------------------------------------- | :--------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01  | O diagrama apresenta corretamente um estado inicial e pelo menos um estado final conforme a notação UML?                  |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF); [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml)             |
| 02  | Os estados identificados (ATIVA, EM_ANDAMENTO, CONCLUIDA, CANCELADA) representam fases reais do ciclo de vida do sistema? |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 03  | Todos os estados possuem ao menos uma transição de entrada ou saída válida?                                               |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                                                           |
| 04  | Não existem estados inalcançáveis ou isolados no fluxo modelado?                                                          |            | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml)                                                                      |

---

## Tabela 2: Verificação das Transições, Eventos e Guardas

| ID  | Pergunta de Verificação                                                                          | Verificado | Rastreabilidade                                                                                                                                                   |
| --- | ------------------------------------------------------------------------------------------------ | :--------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01  | Todas as transições possuem evento explicitamente identificado?                                  |            | [UML Diagrams](https://www.uml-diagrams.org/state-machine-diagrams.html)                                                                                          |
| 02  | As condições de guarda estão corretamente representadas entre colchetes (`[ ]`)?                 |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                                                           |
| 03  | As ações associadas às transições estão descritas após a barra (`/`) conforme padrão UML?        |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                                                           |
| 04  | O cancelamento durante EM_ANDAMENTO representa corretamente um incidente ou interrupção crítica? |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 05  | A chegada ao destino gera corretamente as ações liberar avaliação?                               |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 06  | As transições evitam ambiguidades ou múltiplos caminhos conflitantes para o mesmo evento?        |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                                                           |
| 07  | O fluxo impede que uma carona concluída retorne para estados anteriores?                         |            | Consistência comportamental                                                                                                                                       |

---

## Tabela 3: Verificação da Consistência do Fluxo Comportamental

| ID  | Pergunta de Verificação                                                                | Verificado | Rastreabilidade                                                                                                                                                   |
| --- | -------------------------------------------------------------------------------------- | :--------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01  | O fluxo principal (ATIVA → EM_ANDAMENTO → CONCLUIDA) está claramente representado?     |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 02  | A modelagem diferencia corretamente cancelamento antes e durante a execução da carona? |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 03  | O estado CONCLUIDA representa corretamente o encerramento normal do ciclo da carona?   |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 04  | O estado CANCELADA representa corretamente um encerramento excepcional?                |            | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 05  | O diagrama cobre todos os cenários principais previstos no domínio da aplicação?       |            | Análise geral                                                                                                                                                     |

---

## Conclusão

A verificação do Diagrama de Estados é fundamental para assegurar que o comportamento do sistema esteja modelado de forma consistente com os requisitos e com as regras de negócio do sistema.

O artefato organiza critérios que permitem revisar sistematicamente os estados, as transições, as condições de guarda e as ações associadas, contribuindo para reduzir ambiguidades e inconsistências antes da validação final do modelo.

Dessa forma, o documento fortalece a qualidade da modelagem comportamental do projeto **Carona Amiga FCTE**, servindo como instrumento de apoio à análise técnica e à tomada de decisão da equipe.

## Bibliografia

> 1. OBJECT MANAGEMENT GROUP (OMG). **Unified Modeling Language (UML) Specification – Version 2.5.1**. 2017.  
>    Disponível em: https://www.omg.org/spec/UML/2.5.1/PDF  
>    Acesso em: 23 abr. 2026.

> 2. UML-DIAGRAMS. **State Machine Diagrams Overview**.  
>    Disponível em: https://www.uml-diagrams.org/state-machine-diagrams.html  
>    Acesso em: 23 abr. 2026.

> 3. UML-DIAGRAMS. **State Machine Diagram Elements**.  
>    Disponível em: https://www.uml-diagrams.org/state-machine-diagrams-reference.html  
>    Acesso em: 23 abr. 2026.

> 4. VISUAL PARADIGM. **What is a State Machine Diagram?**  
>    Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-state-machine-diagram/  
>    Acesso em: 23 abr. 2026.

> 5. LUCID SOFTWARE INC. **O que é um Diagrama de Máquina de Estados UML?**  
>    Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml  
>    Acesso em: 23 abr. 2026.

> 6. SPARX SYSTEMS. **UML State Machine Diagram Tutorial**.  
>    Disponível em: https://sparxsystems.com/resources/tutorials/uml2/state-diagram.html  
>    Acesso em: 23 abr. 2026.

## Histórico de Versões

| Versão |    Data    | Descrição                                                             | Autor(es)                                                              | Revisor(es)                                                 | Detalhes da revisão |
| :----: | :--------: | --------------------------------------------------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------- | :-----------------: |
|  1.0   | 23/04/2026 | Elaboração do artefato de verificação alinhado ao Diagrama de Estados | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [João Vitor Santos de Oliveira](https://github.com/Jauzimm) |  Artefato revisado  |
