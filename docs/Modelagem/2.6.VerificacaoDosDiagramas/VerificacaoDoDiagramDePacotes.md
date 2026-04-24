# Verificação do Diagrama de Pacotes

## Introdução

O Diagrama de Pacotes, conforme definido pela UML, é utilizado para organizar e estruturar elementos do sistema em agrupamentos lógicos, evidenciando dependências, separação de responsabilidades e organização arquitetural.

No projeto **Carona Amiga FCTE**, o Diagrama de Pacotes foi elaborado para representar a organização estrutural do sistema em dois grandes módulos: **Backend** e **Frontend**, cada um contendo seus respectivos subpacotes organizados por responsabilidade.

O Backend apresenta uma organização inspirada em princípios de Arquitetura Limpa e separação em camadas, contendo pacotes como `controllers`, `services`, `interfaces service`, `domain`, `ports`, `adapters`, `dto`, `model` e `mapper`.

O Frontend apresenta organização modular baseada em responsabilidades de interface, contendo pacotes como `app`, `components`, `pages`, `routes`, `services`, `context`, `utils` e `assets`.

A verificação deste diagrama é essencial para garantir que a estrutura modular esteja coerente, desacoplada e alinhada às boas práticas arquiteturais.

---

## Objetivo da Verificação

O objetivo da verificação do Diagrama de Pacotes é assegurar que a organização estrutural do sistema esteja:

- Correta do ponto de vista da notação UML;
- Coerente com os princípios de modularização;
- Consistente com a separação de responsabilidades entre Backend e Frontend;
- Livre de dependências cíclicas indevidas;
- Alinhada com boas práticas arquiteturais.

---

## Metodologia

A metodologia de verificação foi conduzida a partir:

- Da análise estrutural do Diagrama de Pacotes.
- Da identificação das dependências entre pacotes.
- Da avaliação da separação entre Backend e Frontend.
- Da especificação UML 2.5.1 (OMG).

Foram observados quatro aspectos principais:

1. Correção da notação UML.
2. Coerência das dependências.
3. Separação adequada de responsabilidades.
4. Ausência de acoplamento indevido entre camadas.

---

## Tabela 1: Verificação da Estrutura Geral e Notação

<font size="3"><p style="text-align: center">Tabela 1: Verificação do Diagrama de Pacotes</p></font>

| ID  | Pergunta de Verificação                                                             | Verificado | Rastreabilidade                                                    |
| --- | ----------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------ |
| 01  | O diagrama utiliza corretamente a notação de pacotes conforme definido pela UML?    | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |
| 02  | Os pacotes Backend e Frontend estão claramente delimitados?                         | Verificado | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 03  | Os subpacotes estão corretamente contidos dentro de seus respectivos módulos?       | Verificado | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 04  | As dependências entre pacotes estão representadas por setas tracejadas apropriadas? | Verificado | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 05  | O diagrama evita poluição visual e mantém legibilidade estrutural?                  | Verificado | Análise estrutural                                                 |

<font size="2"><p style="text-align: center">Fonte: [João Vitor Santos de Oliveira](https://github.com/Jauzimm), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) 2026.</p></font>

---

## Tabela 2: Verificação do Backend

<font size="3"><p style="text-align: center">Tabela 2: Verificação do Diagrama de Pacotes</p></font>

| ID  | Pergunta de Verificação                                                                                   | Verificado | Rastreabilidade                                                    |
| --- | --------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------ |
| 01  | O pacote `controllers` depende apenas de camadas de serviço e não acessa diretamente `domain` ou `model`? | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |
| 02  | O pacote `services` centraliza regras de negócio e coordena acesso ao domínio?                            | Verificado | Análise arquitetural                                               |
| 03  | O pacote `domain` está desacoplado de camadas externas como `controllers`?                                | Verificado | Princípios de Arquitetura Limpa                                    |
| 04  | O pacote `ports` define contratos e evita dependência direta de infraestrutura?                           | Verificado | Princípios de Arquitetura Hexagonal                                |
| 05  | O pacote `adapters` implementa dependências externas respeitando as `ports`?                              | Verificado | Princípios de Arquitetura Hexagonal                                |
| 06  | Não existem dependências cíclicas entre pacotes do Backend?                                               | Verificado | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |

<font size="2"><p style="text-align: center">Fonte: [João Vitor Santos de Oliveira](https://github.com/Jauzimm), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) 2026.</p></font>

---

## Tabela 3: Verificação do Frontend

<font size="3"><p style="text-align: center">Tabela 3: Verificação do Diagrama de Pacotes</p></font>

| ID  | Pergunta de Verificação                                                                 | Verificado | Rastreabilidade                                         |
| --- | --------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------- |
| 01  | O pacote `components` é reutilizável e independente de `pages`?                         | Verificado | Boas práticas de Frontend                               |
| 02  | O pacote `pages` organiza as telas principais sem concentrar regras de negócio?         | Verificado | Análise estrutural                                      |
| 03  | O pacote `services` é responsável pela comunicação com o Backend?                       | Verificado | Arquitetura em camadas                                  |
| 04  | O pacote `context` centraliza gerenciamento de estado global?                           | Verificado | Padrão Context API                                      |
| 05  | O pacote `utils` contém funções auxiliares desacopladas da camada de interface?         | Verificado | Boas práticas de modularização                          |
| 06  | Não existem dependências cruzadas inadequadas entre `components`, `pages` e `services`? | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF) |

<font size="2"><p style="text-align: center">Fonte: [João Vitor Santos de Oliveira](https://github.com/Jauzimm), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) 2026.</p></font>

---

## Tabela 4: Verificação da Integração Backend–Frontend

<font size="3"><p style="text-align: center">Tabela 4: Verificação do Diagrama de Pacotes</p></font>

| ID  | Pergunta de Verificação                                                                    | Verificado | Rastreabilidade                                                    |
| --- | ------------------------------------------------------------------------------------------ | :--------: | ------------------------------------------------------------------ |
| 01  | A comunicação entre Frontend e Backend ocorre exclusivamente por meio dos `services`?      | Verificado | Arquitetura Cliente-Servidor                                       |
| 02  | Não existem dependências diretas estruturais entre pacotes internos do Backend e Frontend? | Verificado | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 03  | O diagrama mantém clara separação de responsabilidades entre as camadas?                   | Verificado | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |

<font size="2"><p style="text-align: center">Fonte: [João Vitor Santos de Oliveira](https://github.com/Jauzimm), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) 2026.</p></font>

---

## Conclusão

A verificação do Diagrama de Pacotes permite avaliar a organização estrutural do sistema sob a perspectiva arquitetural, assegurando modularidade, baixo acoplamento e clareza de responsabilidades.

O artefato organiza critérios objetivos que auxiliam na identificação de dependências inadequadas, violações de camadas e possíveis ciclos estruturais, contribuindo para a melhoria da qualidade arquitetural do projeto **Carona Amiga FCTE**.

Dessa forma, o documento atua como instrumento de apoio à validação técnica da organização modular do sistema.

---

## Vídeo de Verificação do Diagrama de Pacotes

A gravação do vídeo de verificação serviu para validar o modelo desenvolvido, tomando como referência as questões de verificação para detectar falhas e inconsistências. Na sessão de gravação, foram abordados os aspectos positivos do diagrama, além das regiões que requeriam melhorias.

<iframe width="560" height="315" src="https://www.youtube.com/embed/y0RPgiCZZsA?si=GGyptvlUrCeQjjJ-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://www.youtube.com/watch?v=y0RPgiCZZsA" target="_blank">Clique aqui para assistir no YouTube</a></p>

<font size="2"><p style="text-align: center">Fonte: [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

## Bibliografia

> 1. OBJECT MANAGEMENT GROUP (OMG). **Unified Modeling Language (UML) Specification – Version 2.5.1**. 2017. Disponível em: https://www.omg.org/spec/UML/2.5.1/PDF. Acesso em: 23 abr. 2026.

> 2. UML-DIAGRAMS. **Package Diagrams Overview**. Disponível em: [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html). Acesso em: 23 abr. 2026.

> 3. UML-DIAGRAMS. **Package Diagram Reference**. Disponível em: https://www.uml-diagrams.org/package-diagrams-reference.html. Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                    | Autor(es)                                                              | Revisor(es) | Detalhes da revisão |
| :----: | :--------: | ------------------------------------------------------------ | ---------------------------------------------------------------------- | ----------- | :-----------------: |
|  1.0   | 23/04/2026 | Elaboração do artefato de verificação do Diagrama de Pacotes | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) e [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss)| [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) |  Artefato Revisado  |
