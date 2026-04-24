# Verificação do Diagrama de Componentes

## Introdução

Conforme definido pela documentação oficial da UML [[1]](#ref1), o Diagrama de Componentes é um diagrama estrutural que descreve a organização física dos módulos de software, suas **interfaces providas e requeridas** e as **dependências** entre subsistemas. Diferentemente do diagrama de classes, que modela a estrutura lógica, o diagrama de componentes foca nos blocos de construção executáveis ou implantáveis do sistema — como bibliotecas, serviços e módulos — e nos contratos (interfaces) que estes estabelecem entre si.

No projeto **Carona Amiga FCTE**, o Diagrama de Componentes foi elaborado para evidenciar os subsistemas principais (`Backend`, `Client`, `Chat`, `Rating`, `Profile` e `Authentication`), seus contratos de comunicação e as dependências entre eles, apoiando decisões de arquitetura e facilitando a manutenção do sistema.

A verificação desse diagrama é essencial para garantir que os componentes modelados estejam corretos, completos e aderentes à notação UML, e que as dependências e interfaces representem fielmente a arquitetura planejada para o sistema.

---

## Objetivo da Verificação

O objetivo da verificação do Diagrama de Componentes é garantir que o modelo arquitetural esteja correto, completo e consistente com os requisitos do sistema. Busca-se:

- Verificar se os componentes estão corretamente nomeados e identificados com estereótipos UML adequados.
- Avaliar se as interfaces providas e requeridas estão corretamente representadas pela notação bola-e-soquete.
- Confirmar se as dependências entre componentes e subsistemas são coerentes com a arquitetura do sistema.
- Identificar componentes sem interfaces definidas, subsistemas mal delimitados ou relacionamentos ausentes.
- Garantir aderência às convenções UML para diagramas de componentes.

---

## Metodologia de Verificação

A metodologia de verificação foi conduzida a partir:

- Da análise do [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md) elaborado pela equipe.
- Dos requisitos funcionais e não funcionais consolidados na Entrega 01 do projeto.
- Da especificação UML 2.5.1 (OMG) e materiais de referência sobre modelagem de componentes.

Foram observados quatro aspectos principais:

1. Correção da notação UML dos componentes e subsistemas.
2. Adequação das interfaces providas e requeridas.
3. Consistência e completude das dependências entre componentes.
4. Alinhamento com os requisitos arquiteturais do sistema.

Com essa metodologia, foram criadas perguntas baseadas nas referências bibliográficas para guiar a verificação do Diagrama de Componentes, depois gravamos em conjunto para validar o diagrama e corrigir possíveis erros antes da entrega final.

---

## Tabela 1: Verificação dos Componentes e Estrutura Geral

<font size="3"><p style="text-align: center">Tabela 1: Verificação dos Componentes e Estrutura Geral</p></font>

| ID  | Pergunta de Verificação                                                                                                                         | Verificado | Rastreabilidade                                                                                                          |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------------------------------------------------------------ |
| 01  | Todos os componentes estão identificados com o estereótipo `<<component>>` ou o ícone padrão UML?                                               | Verificado | [UML Diagrams](https://www.uml-diagrams.org/component-diagrams.html)                                                    |
| 02  | Os nomes dos componentes são substantivos ou expressões nominais que representam módulos coesos do sistema?                                     | Verificado | [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/)       |
| 03  | Os seis subsistemas (`Backend`, `Client`, `Chat`, `Rating`, `Profile` e `Authentication`) estão delimitados com o estereótipo `<<subsystem>>`?  | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                 |
| 04  | O subsistema `Backend` contém corretamente os componentes `:LocationService`, `:Ride Api`, `:Api Principal`, `:Notification Service` e `:AuthService`? | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                      |
| 05  | O subsistema `Client` contém corretamente os componentes `:App Driver`, `:App Passager` e `:Api Mobile`?                                        | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                           |
| 06  | O subsistema `Authentication` contém corretamente os componentes `:Login`, `:Cadaster` e `:Recover Password`?                                   | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                           |
| 07  | Os subsistemas `Chat`, `Rating` e `Profile` contêm, respectivamente, `:Chat Service`, `:Rating Api` e `:Profile Api` como únicos componentes?  | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                           |
| 08  | O `:Api Principal` está representado como componente central de roteamento dentro do subsistema `Backend`?                                      | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                           |
| 09  | Cada componente possui responsabilidade claramente delimitada e não sobrepõe a responsabilidade de outro componente?                            | Verificado | [GeeksforGeeks](https://www.geeksforgeeks.org/component-diagram-unified-modeling-language-uml/)                          |
| 10  | Portas de interação estão representadas corretamente como pequenos quadrados na borda dos componentes?                                          | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                                 |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Tabela 2: Verificação das Interfaces Providas e Requeridas

<font size="3"><p style="text-align: center">Tabela 2: Verificação das Interfaces Providas e Requeridas</p></font>

| ID  | Pergunta de Verificação                                                                                                                                    | Verificado | Rastreabilidade                                                                                                    |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------------------------------------------------------ |
| 01  | As interfaces providas estão representadas com o símbolo de bola (círculo sólido) conforme a notação bola-e-soquete?                                       | Verificado | [UML Diagrams](https://www.uml-diagrams.org/component-diagrams.html)                                              |
| 02  | As interfaces requeridas estão representadas com o símbolo de soquete (semicírculo aberto) conforme a notação bola-e-soquete?                              | Verificado | [UML Diagrams](https://www.uml-diagrams.org/component-diagrams.html)                                              |
| 03  | Todas as interfaces possuem nomes que descrevem claramente o contrato que estabelecem?                                                                     | Verificado | [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/) |
| 04  | A `Location Interface` está corretamente provida por `:LocationService` e consumida pelo subsistema `Client`?                                              | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 05  | A `Ride Interface` está corretamente provida por `:Ride Api` e consumida pelos componentes `:App Driver` e `:App Passager`?                                | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 06  | A `Authentication Interface` está corretamente provida por `:AuthService` e consumida pelo subsistema `Client` via `:Api Mobile`?                          | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 07  | A `Chat Interface` está corretamente provida por `:Chat Service` e consumida pelo subsistema `Client`?                                                     | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 08  | A `Rating Interface` está corretamente provida por `:Rating Api` e consumida pelo subsistema `Client`?                                                     | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 09  | A `Profile Interface` está corretamente provida por `:Profile Api` e consumida pelo subsistema `Client`?                                                   | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 10  | Os conectores de montagem ligam corretamente a interface provida de um componente à interface requerida do componente consumidor em todos os casos?         | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                           |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Tabela 3: Verificação dos Relacionamentos e Dependências

<font size="3"><p style="text-align: center">Tabela 3: Verificação dos Relacionamentos e Dependências</p></font>

| ID  | Pergunta de Verificação                                                                                                                                      | Verificado | Rastreabilidade                                                                                                    |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | :--------: | ------------------------------------------------------------------------------------------------------------------ |
| 01  | As dependências entre componentes estão representadas com linhas tracejadas e seta (`- - - - ►`) apontando para o componente dependido?                      | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)                                                           |
| 02  | A dependência rotulada `Create User` entre `:AuthService` e `:Cadaster` possui semântica de negócio coerente com o fluxo de cadastro do sistema?             | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 03  | A dependência rotulada `Validate User` entre `:AuthService` e `:Login` possui semântica de negócio coerente com o fluxo de autenticação do sistema?          | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 04  | A dependência rotulada `Recovery Password` entre `:AuthService` e `:Recover Password` está corretamente representada e semanticamente coerente?              | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 05  | Não existem dependências circulares não justificadas entre componentes do mesmo subsistema?                                                                  | Verificado | [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/) |
| 06  | O `:Notification Service` está conectado ao fluxo de eventos do sistema de forma coerente com sua responsabilidade dentro do `Backend`?                     | Verificado | [Diagrama de Componentes](../2.1.ModelagemEstatica/Diagrama_de_componentes.md)                                     |
| 07  | Todos os componentes do diagrama participam de ao menos uma relação (provendo ou consumindo uma interface, ou possuindo uma dependência rotulada)?            | Verificado | [GeeksforGeeks](https://www.geeksforgeeks.org/component-diagram-unified-modeling-language-uml/)                    |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Verificação do Diagrama de Componentes

A verificação do Diagrama de Componentes foi realizada de forma assíncrona, com cada membro da equipe analisando individualmente o diagrama com base nas perguntas de verificação elaboradas. Cada integrante revisou os componentes, subsistemas, interfaces e dependências de forma independente, registrando suas observações e identificando possíveis inconsistências. As conclusões foram posteriormente consolidadas pela equipe, garantindo que todos os critérios de verificação fossem devidamente avaliados antes da entrega final do artefato.

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Conclusão

A verificação do Diagrama de Componentes é fundamental para assegurar que a arquitetura do sistema **Carona Amiga FCTE** esteja modelada de forma consistente com os requisitos e as boas práticas da UML. O artefato organiza critérios que permitem revisar sistematicamente os componentes, os subsistemas, as interfaces providas e requeridas, e as dependências entre os módulos.

Ao seguir uma metodologia estruturada de verificação, é possível identificar e corrigir erros, como componentes sem interfaces definidas, dependências incorretas ou subsistemas mal delimitados, garantindo que o modelo seja uma representação fiel da arquitetura planejada. Em última análise, a verificação do Diagrama de Componentes contribui para o alinhamento arquitetural da equipe e para a rastreabilidade entre requisitos e implementação.

---

## Referências Bibliográficas

> 1. OBJECT MANAGEMENT GROUP (OMG). **Unified Modeling Language (UML) Specification – Version 2.5.1**. 2017.  
>    Disponível em: https://www.omg.org/spec/UML/2.5.1/PDF  
>    Acesso em: 23 abr. 2026.

> 2. UML DIAGRAMS. **Component Diagrams Overview**.  
>    Disponível em: https://www.uml-diagrams.org/component-diagrams.html  
>    Acesso em: 23 abr. 2026.

> 3. VISUAL PARADIGM. **What is Component Diagram?**  
>    Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/  
>    Acesso em: 23 abr. 2026.

> 4. GEEKSFORGEEKS. **Component Diagram – Unified Modeling Language (UML)**.  
>    Disponível em: https://www.geeksforgeeks.org/component-diagram-unified-modeling-language-uml/  
>    Acesso em: 23 abr. 2026.

> 5. LUCIDCHART. **O que é um Diagrama de Componentes UML?**  
>    Disponível em: https://www.lucidchart.com/pages/pt/diagrama-de-componentes-uml  
>    Acesso em: 23 abr. 2026.

> 6. SPARX SYSTEMS. **UML Component Diagram Tutorial**.  
>    Disponível em: https://sparxsystems.com/resources/tutorials/uml2/component-diagram.html  
>    Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                                  | Autor(es)                                                                                                                                                                                                               | Revisor(es)                                                             | Detalhes da revisão         |
| :----: | :--------: | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | :-------------------------: |
|  1.0   | 24/04/2026 | Criação do artefato de verificação do Diagrama de Componentes              | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | Estrutura inicial e checklists de verificação |
