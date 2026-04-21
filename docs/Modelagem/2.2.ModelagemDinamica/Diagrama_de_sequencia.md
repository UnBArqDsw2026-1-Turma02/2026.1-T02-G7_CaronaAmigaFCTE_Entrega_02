# Diagrama de Sequência

## Introdução

O diagrama de sequência é um dos principais artefatos da UML utilizados para representar o comportamento dinâmico de um sistema, evidenciando a troca de mensagens entre seus elementos ao longo do tempo. De acordo com a Apostila UML <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-1">[1]</a>, esse tipo de diagrama descreve, de forma visual e cronológica, como ocorre a interação entre atores e objetos envolvidos na execução de uma funcionalidade específica.

A estrutura de um diagrama de sequência é organizada em dois eixos principais: o eixo vertical, que representa o tempo (de cima para baixo), e o eixo horizontal, que apresenta os participantes da interação, cada um com sua respectiva linha de vida. As mensagens trocadas entre esses elementos são representadas por setas, permitindo visualizar com clareza a ordem das operações e a comunicação entre os componentes do sistema, conforme descrito pela IBM <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>.

No contexto do projeto **Carona Amiga FCTE**, os diagramas de sequência são utilizados para detalhar as interações entre os usuários, especialmente passageiros e motoristas — e os componentes internos da aplicação, como interface, APIs, serviços e banco de dados. Esses diagramas complementam os modelos estruturais previamente desenvolvidos, como os diagramas de classes e de componentes, garantindo consistência entre a arquitetura do sistema e seu comportamento em tempo de execução.

Dessa forma, a modelagem por meio de diagramas de sequência contribui para o entendimento dos fluxos principais da aplicação, como cadastro, autenticação, busca de caronas, solicitação de participação e gerenciamento de viagens. Além disso, auxilia na identificação de responsabilidades, na validação dos requisitos e no suporte às etapas de implementação e manutenção do sistema.

---

## Objetivos

O objetivo desta seção é apresentar os diagramas de sequência do sistema **Carona Amiga FCTE**, modelando as principais interações entre os atores e os componentes internos da aplicação. A partir desses diagramas, busca-se:

- Modelar visualmente o fluxo de mensagens entre usuários e sistema;
- Evidenciar a ordem temporal das interações durante a execução das funcionalidades;
- Identificar as responsabilidades dos componentes envolvidos em cada processo;
- Ilustrar o comportamento dinâmico da aplicação com base nos casos de uso definidos;
- Apoiar o entendimento do funcionamento interno do sistema em tempo de execução;
- Contribuir para a validação dos requisitos e para a coerência entre os modelos de análise e projeto.

De forma mais específica, os diagramas desenvolvidos visam representar cenários centrais do sistema **Carona Amiga FCTE**, tais como:

- **Cadastro de usuário**: criação de conta na plataforma;
- **Login**: autenticação do usuário no sistema;
- **Busca de caronas**: consulta de caronas disponíveis com base em filtros;
- **Solicitação de participação em carona**: envio de solicitação do passageiro ao motorista;
- **Publicação de carona**: cadastro de uma nova viagem pelo motorista;
- **Confirmação de embarque**: validação da participação do passageiro na carona.

Esses cenários foram escolhidos por representarem as funcionalidades essenciais da aplicação, permitindo uma visão clara e detalhada das interações entre os atores e os módulos do sistema.


---

## Metodologia

---

## Referências bibliográficas

> <a id="referencias-bibliograficas-1">1.</a> APOSTILA UML. **Unified Modeling Language – Linguagem de Modelagem Unificada em Português**. Seção sobre diagrama de sequência. Disponibilizada pela professora. Acesso em: 30 abr. 2025.  

> <a id="referencias-bibliograficas-2">2.</a> IBM. **Diagramas de Sequência**. Disponível em: https://www.ibm.com/docs/pt-br/rsm/7.5.0?topic=uml-sequence-diagrams. Acesso em: 30 abr. 2025.  

---

## Histórico de versão

Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da Revisão
-------|------|-----------|-----------|-------------|-----------------
1.0 | 21/04/2026 | Criação do artefato |[Ana Victória Guedes da Costa](https://github.com/navicg) | [Karoline Luz da Conceição](https://github.com/KarolineLuz)| Artefato revisado