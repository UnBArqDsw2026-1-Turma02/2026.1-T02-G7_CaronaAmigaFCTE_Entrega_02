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

| ID  | Pergunta de Verificação                                                             | Verificado | Rastreabilidade                                                    |
| --- | ----------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------ |
| 01  | O diagrama utiliza corretamente a notação de pacotes conforme definido pela UML?    |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |
| 02  | Os pacotes Backend e Frontend estão claramente delimitados?                         |            | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 03  | Os subpacotes estão corretamente contidos dentro de seus respectivos módulos?       |            | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 04  | As dependências entre pacotes estão representadas por setas tracejadas apropriadas? |            | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 05  | O diagrama evita poluição visual e mantém legibilidade estrutural?                  |            | Análise estrutural                                                 |

---

## Tabela 2: Verificação do Backend

| ID  | Pergunta de Verificação                                                                                   | Verificado | Rastreabilidade                                                    |
| --- | --------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------------------ |
| 01  | O pacote `controllers` depende apenas de camadas de serviço e não acessa diretamente `domain` ou `model`? |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |
| 02  | O pacote `services` centraliza regras de negócio e coordena acesso ao domínio?                            |            | Análise arquitetural                                               |
| 03  | O pacote `domain` está desacoplado de camadas externas como `controllers`?                                |            | Princípios de Arquitetura Limpa                                    |
| 04  | O pacote `ports` define contratos e evita dependência direta de infraestrutura?                           |            | Princípios de Arquitetura Hexagonal                                |
| 05  | O pacote `adapters` implementa dependências externas respeitando as `ports`?                              |            | Princípios de Arquitetura Hexagonal                                |
| 06  | Não existem dependências cíclicas entre pacotes do Backend?                                               |            | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |

---

## Tabela 3: Verificação do Frontend

| ID  | Pergunta de Verificação                                                                 | Verificado | Rastreabilidade                                         |
| --- | --------------------------------------------------------------------------------------- | :--------: | ------------------------------------------------------- |
| 01  | O pacote `components` é reutilizável e independente de `pages`?                         |            | Boas práticas de Frontend                               |
| 02  | O pacote `pages` organiza as telas principais sem concentrar regras de negócio?         |            | Análise estrutural                                      |
| 03  | O pacote `services` é responsável pela comunicação com o Backend?                       |            | Arquitetura em camadas                                  |
| 04  | O pacote `context` centraliza gerenciamento de estado global?                           |            | Padrão Context API                                      |
| 05  | O pacote `utils` contém funções auxiliares desacopladas da camada de interface?         |            | Boas práticas de modularização                          |
| 06  | Não existem dependências cruzadas inadequadas entre `components`, `pages` e `services`? |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF) |

---

## Tabela 4: Verificação da Integração Backend–Frontend

| ID  | Pergunta de Verificação                                                                    | Verificado | Rastreabilidade                                                    |
| --- | ------------------------------------------------------------------------------------------ | :--------: | ------------------------------------------------------------------ |
| 01  | A comunicação entre Frontend e Backend ocorre exclusivamente por meio dos `services`?      |            | Arquitetura Cliente-Servidor                                       |
| 02  | Não existem dependências diretas estruturais entre pacotes internos do Backend e Frontend? |            | [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) |
| 03  | O diagrama mantém clara separação de responsabilidades entre as camadas?                   |            | [OMG UML 2.5.1](https://www.omg.org/spec/UML/2.5.1/PDF)            |

---

## Conclusão

A verificação do Diagrama de Pacotes permite avaliar a organização estrutural do sistema sob a perspectiva arquitetural, assegurando modularidade, baixo acoplamento e clareza de responsabilidades.

O artefato organiza critérios objetivos que auxiliam na identificação de dependências inadequadas, violações de camadas e possíveis ciclos estruturais, contribuindo para a melhoria da qualidade arquitetural do projeto **Carona Amiga FCTE**.

Dessa forma, o documento atua como instrumento de apoio à validação técnica da organização modular do sistema.

---

## Bibliografia

> 1. OBJECT MANAGEMENT GROUP (OMG). **Unified Modeling Language (UML) Specification – Version 2.5.1**. 2017.  
>    Disponível em: https://www.omg.org/spec/UML/2.5.1/PDF  
>    Acesso em: 23 abr. 2026.

> 2. UML-DIAGRAMS. **Package Diagrams Overview**.  
>    Disponível em: [UML-Diagrams](https://www.uml-diagrams.org/package-diagrams.html) Acesso em: 23 abr. 2026.

> 3. UML-DIAGRAMS. **Package Diagram Reference**.  
>    Disponível em: https://www.uml-diagrams.org/package-diagrams-reference.html  
>    Acesso em: 23 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                                                    | Autor(es)                                                              | Revisor(es) | Detalhes da revisão |
| :----: | :--------: | ------------------------------------------------------------ | ---------------------------------------------------------------------- | ----------- | :-----------------: |
|  1.0   | 23/04/2026 | Elaboração do artefato de verificação do Diagrama de Pacotes | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) |             |                     |
