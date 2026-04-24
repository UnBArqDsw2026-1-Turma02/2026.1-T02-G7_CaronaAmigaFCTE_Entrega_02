# Verificação do Diagrama de Atividades

## Introdução

O Diagrama de Atividades, conforme definido pela UML, é um diagrama comportamental utilizado para descrever o fluxo de controle ou o fluxo de dados de um sistema, detalhando a sequência lógica de passos, decisões e condições de um processo de negócio ou algoritmo. Diferente de outros diagramas que focam em *quem* realiza as ações, o foco do Diagrama de Atividades está em *o que* acontece e em *qual ordem*.

No projeto **Carona Amiga FCTE**, o Diagrama de Atividades foi elaborado com o uso de *Swimlanes* (raias) para organizar as responsabilidades e fluxos principais do sistema, permitindo visualizar processos complexos como login, cadastro, oferta de carona, pedido de carona e avaliação dos usuários.

A verificação desse diagrama é fundamental para garantir que os fluxos modelados estejam coerentes com as regras de negócio, que as decisões representem corretamente os pontos de desvio do sistema e que não existam inconsistências comportamentais ou fluxos sem encerramento.

---

## Objetivo da Verificação

O objetivo da verificação do Diagrama de Atividades é garantir que o modelo comportamental do sistema esteja correto, completo e consistente com os requisitos do sistema.

Busca-se:

- Verificar se os elementos do diagrama utilizam a notação UML correta (nó inicial, atividades, decisões, nó final).
- Avaliar se os fluxos de controle representam adequadamente as sequências lógicas dos processos do sistema.
- Confirmar se as *Swimlanes* delimitam corretamente as responsabilidades de cada domínio funcional.
- Identificar possíveis fluxos mortos, decisões sem caminhos alternativos ou atividades isoladas.
- Garantir aderência às convenções UML para Diagramas de Atividades.

---

## Metodologia

A metodologia de verificação foi conduzida a partir:

- Da análise do [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md) elaborado pela equipe.
- Dos requisitos funcionais relacionados aos fluxos de login, cadastro, oferta de carona, pedido de carona e avaliação.
- Da especificação UML 2.5.1 (OMG) e materiais de referência sobre modelagem de atividades.

Foram observados quatro aspectos principais:

1. Correção da notação UML dos elementos do diagrama.
2. Coerência e completude do fluxo de controle entre as atividades.
3. Consistência das regras de negócio e dos pontos de decisão.
4. Adequação do uso de *Swimlanes* para organização dos domínios funcionais.

---

## Tabela 1: Verificação dos Elementos e Notação UML

<font size="3"><p style="text-align: center">Tabela 1: Verificação dos Elementos e Notação UML</p></font>

| ID  | Pergunta de Verificação                                                                                                                          | Verificado | Rastreabilidade                                                                                       |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------ | :--------: | ----------------------------------------------------------------------------------------------------- |
| 01  | Cada uma das cinco *Swimlanes* (`Fazer login`, `Cadastrar Conta`, `Oferecer carona`, `Pedir Carona` e `Avaliação`) possui exatamente um nó inicial (círculo preto sólido)? | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF) |
| 02  | Os nós finais de atividade estão representados com o símbolo correto (círculo com borda) ao final de cada fluxo?                                | Verificado | [UML Diagrams](https://www.uml-diagrams.org/activity-diagrams.html)                                   |
| 03  | As atividades estão representadas com retângulos de cantos arredondados e possuem nomes que descrevem ações concretas?                          | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-atividades-uml)                  |
| 04  | Os pontos de decisão estão representados com losangos e possuem ao menos duas arestas de saída com condições identificadas?                     | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                              |
| 05  | Os fluxos de controle estão representados com setas direcionais que indicam a sequência correta entre as atividades?                            | Verificado | [UML Diagrams](https://www.uml-diagrams.org/activity-diagrams.html)                                   |
| 06  | As cinco *Swimlanes* estão corretamente delimitadas, nomeadas e organizam as atividades de acordo com o domínio funcional correspondente?        | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                          |
| 07  | Não há uso incorreto de outros elementos UML (ex.: estados do Diagrama de Estados) no lugar dos elementos de atividades?                        | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                              |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Tabela 2: Verificação do Fluxo de Controle e Lógica de Negócio

<font size="3"><p style="text-align: center">Tabela 2: Verificação do Fluxo de Controle e Lógica de Negócio</p></font>

| ID  | Pergunta de Verificação                                                                                                                                                                 | Verificado | Rastreabilidade                                                                                                                                                    |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 01  | No fluxo `Fazer login`, as atividades `Preencher e-mail institucional` e `Preencher a senha` estão representadas como caminhos paralelos que convergem corretamente antes do nó final? | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 02  | No fluxo `Cadastrar Conta`, a decisão `Dados verificados?` com resultado `Não` retorna corretamente à atividade `Inserir nome, e-mail, matrícula e senha`, formando um laço de correção? | Verificado | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 03  | Nos fluxos `Oferecer carona`, `Pedir Carona` e `Avaliação`, a decisão `Fazer login na conta` está presente como pré-condição de acesso à funcionalidade principal?                     | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 04  | No fluxo `Oferecer carona`, a atividade `Informar preço da carona` está corretamente conectada como entrada para a atividade `Publicar carona`?                                        | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 05  | No fluxo `Oferecer carona`, a decisão após `Aceitar passageiros` com resultado `Sim` leva corretamente a `Realizar carona` e ao nó final?                                              | Verificado | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 06  | No fluxo `Pedir Carona`, a decisão `Esperar notificação do motorista` separa corretamente os caminhos `Pedido aceito` (→ `Abrir chat` / `Visualizar carona`) e `Pedido recusado` (→ retorno a `Selecionar carona`)? | Verificado | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 07  | No fluxo `Pedir Carona`, a atividade `Viagem realizada` encerra corretamente o fluxo no nó final após a confirmação de embarque?                                                       | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 08  | No fluxo `Avaliação`, a decisão `Possui viagens passadas?` com resultado `Não` conduz diretamente ao nó final, impedindo acesso à avaliação sem histórico de viagens?                 | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 09  | No fluxo `Avaliação`, o caminho `Sim` leva sequencialmente a `Ver histórico` → `Selecionar viagem` → decisão `Denunciar a viagem` → `Avalie essa viagem` → nó final?                 | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 10  | Todos os caminhos de decisão convergem corretamente para atividades subsequentes ou nós finais, sem fluxos suspensos em nenhuma das cinco *Swimlanes*?                                 | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                                                           |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Tabela 3: Verificação da Consistência e Completude do Diagrama

<font size="3"><p style="text-align: center">Tabela 3: Verificação da Consistência e Completude do Diagrama</p></font>

| ID  | Pergunta de Verificação                                                                                                                              | Verificado | Rastreabilidade                                                                                                                                                    |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 01  | O diagrama cobre os cinco processos principais: `Fazer login`, `Cadastrar Conta`, `Oferecer carona`, `Pedir Carona` e `Avaliação`?                   | Verificado | [Diagrama de Atividades](../2.2.ModelagemDinamica/Diagrama_de_atividades.md)                                                                                       |
| 02  | As condições dos pontos de decisão estão descritas de forma clara e não ambígua (`Sim`/`Não`, `Pedido aceito`/`Pedido recusado`)?                   | Verificado | [Lucidchart](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-atividades-uml)                                                                              |
| 03  | O laço de reentrada do fluxo `Cadastrar Conta` (`Não` → `Inserir nome, e-mail, matrícula e senha`) não configura um ciclo infinito sem condição de saída? | Verificado | [UML Diagrams](https://www.uml-diagrams.org/activity-diagrams.html)                                                                                           |
| 04  | O laço de reentrada do fluxo `Pedir Carona` (`Pedido recusado` → `Selecionar carona`) não configura um ciclo infinito sem condição de saída?        | Verificado | [UML Diagrams](https://www.uml-diagrams.org/activity-diagrams.html)                                                                                               |
| 05  | As atividades representadas no diagrama são consistentes com as funcionalidades identificadas nos requisitos do sistema?                             | Verificado | [Requisitos do sistema](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md) |
| 06  | O nível de granularidade das atividades é adequado — nem excessivamente detalhado nem muito abstrato para o contexto do sistema?                     | Verificado | Análise geral                                                                                                                                                      |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Vídeo de Verificação do Diagrama de Atividades

A verificação do Diagrama de Atividades foi realizada de forma assíncrona, com cada membro da equipe analisando individualmente o diagrama com base nas perguntas de verificação elaboradas. Cada integrante revisou os componentes, subsistemas, interfaces e dependências de forma independente, registrando suas observações e identificando possíveis inconsistências. As conclusões foram posteriormente consolidadas pela equipe, garantindo que todos os critérios de verificação fossem devidamente avaliados antes da entrega final do artefato.

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Conclusão

A verificação do Diagrama de Atividades é fundamental para assegurar que o comportamento funcional do sistema **Carona Amiga FCTE** esteja modelado de forma consistente com os requisitos e com as regras de negócio do sistema.

O artefato organiza critérios que permitem revisar sistematicamente os elementos de notação UML, os fluxos de controle, os pontos de decisão e o uso de *Swimlanes*, contribuindo para reduzir ambiguidades e inconsistências antes da validação final do modelo.

Dessa forma, o documento fortalece a qualidade da modelagem comportamental do projeto **Carona Amiga FCTE**, servindo como instrumento de apoio à análise técnica e à tomada de decisão da equipe na implementação dos fluxos do sistema.

---

## Referências Bibliográficas

> 1. OBJECT MANAGEMENT GROUP (OMG). **Unified Modeling Language (UML) Specification – Version 2.5.1**. 2017.  
>    Disponível em: https://www.omg.org/spec/UML/2.5.1/PDF  
>    Acesso em: 24 abr. 2026.

> 2. UML DIAGRAMS. **Activity Diagrams Overview**.  
>    Disponível em: https://www.uml-diagrams.org/activity-diagrams.html  
>    Acesso em: 24 abr. 2026.

> 3. LUCIDCHART. **O que é um Diagrama de Atividades UML?**  
>    Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-atividades-uml  
>    Acesso em: 24 abr. 2026.

> 4. VISUAL PARADIGM. **What is Activity Diagram?**  
>    Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-activity-diagram/  
>    Acesso em: 24 abr. 2026.

> 5. SERRANO, Milene. **Slides – Diagrama de Atividades UML**.  
>    Disponível em: https://aprender3.unb.br/pluginfile.php/3178534/mod_page/content/1/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Modelagem%20UML%20Din%C3%A2mica%20-%20Profa.%20Milene.pdf  
>    Acesso em: 24 abr. 2026.

> 6. SPARX SYSTEMS. **UML Activity Diagram Tutorial**.  
>    Disponível em: https://sparxsystems.com/resources/tutorials/uml2/activity-diagram.html  
>    Acesso em: 24 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                                  | Autor(es)                                                                                                                                                                                                               | Revisor(es) | Detalhes da revisão                          |
| :----: | :--------: | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | :------------------------------------------: |
|  1.0   | 24/04/2026 | Criação do artefato de verificação do Diagrama de Atividades               | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | —           | Estrutura inicial e checklists de verificação |
