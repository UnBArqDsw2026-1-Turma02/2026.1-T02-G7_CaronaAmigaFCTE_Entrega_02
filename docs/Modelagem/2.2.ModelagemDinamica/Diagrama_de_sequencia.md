# Diagrama de Sequência

## Introdução

O diagrama de sequência é um dos principais artefatos da UML utilizados para representar o comportamento dinâmico de um sistema, evidenciando a troca de mensagens entre seus elementos ao longo do tempo. De acordo com a Apostila UML <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-1">[1]</a>, esse tipo de diagrama descreve, de forma visual e cronológica, como ocorre a interação entre atores e objetos envolvidos na execução de uma funcionalidade específica.

A estrutura de um diagrama de sequência é organizada em dois eixos principais: o eixo vertical, que representa o tempo (de cima para baixo), e o eixo horizontal, que apresenta os participantes da interação, cada um com sua respectiva linha de vida. As mensagens trocadas entre esses elementos são representadas por setas, permitindo visualizar com clareza a ordem das operações e a comunicação entre os componentes do sistema, conforme descrito pela IBM <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>.

No contexto do projeto **Carona Amiga FCTE**, os diagramas de sequência são utilizados para detalhar as interações entre os usuários, especialmente passageiros e motoristas — e os componentes internos da aplicação, como interface, APIs, serviços e banco de dados. Esses diagramas complementam os modelos estruturais previamente desenvolvidos, como os diagramas de classes e de componentes, garantindo consistência entre a arquitetura do sistema e seu comportamento em tempo de execução.

Dessa forma, a modelagem por meio de diagramas de sequência contribui para o entendimento dos fluxos principais da aplicação, como cadastro, autenticação, busca de caronas, solicitação de participação e gerenciamento de viagens. Além disso, auxilia na identificação de responsabilidades, na validação dos requisitos e no suporte às etapas de implementação e manutenção do sistema.

Tomando como base a legenda já elaborada para o projeto e as convenções da UML descritas na bibliografia adotada <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-1">[1]</a> <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>, a leitura dos diagramas considera elementos como participante ou objeto, linha de vida, mensagens síncronas e assíncronas, resposta ou retorno e autochamada. Essa padronização fortalece a rastreabilidade entre a fundamentação teórica, a representação visual utilizada pela equipe e os fluxos modelados para o **Carona Amiga FCTE**.

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

A elaboração dos diagramas de sequência do **Carona Amiga FCTE** seguirá uma abordagem iterativa, com base nos artefatos previamente construídos pela equipe e nos fluxos definidos no protótipo de alta fidelidade da aplicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-3">[3]</a>. A partir desses fluxos, o comportamento do sistema será observado sob a perspectiva temporal das interações, permitindo identificar a ordem das mensagens trocadas entre os atores, a interface, os serviços internos e a persistência dos dados.

Os fluxos trabalhados foram selecionados por representarem funcionalidades centrais da plataforma:

- **Cadastro e autenticação de usuários**: envolve a criação de conta e o login de passageiros e motoristas, permitindo o acesso seguro à aplicação;
- **Busca e visualização de caronas**: representa o fluxo em que o passageiro consulta as caronas disponíveis, aplica filtros e acessa os detalhes de uma viagem;
- **Solicitação de participação em carona**: descreve a interação do passageiro ao enviar uma solicitação para participar de uma carona oferecida;
- **Publicação de carona**: contempla o processo realizado pelo motorista para cadastrar uma nova viagem, informando rota, horário, vagas e demais dados relevantes;
- **Gerenciamento e confirmação de embarque**: representa as interações necessárias para acompanhar solicitações, confirmar participantes e validar a participação do passageiro na carona.

Para a construção dos diagramas, foram consideradas as seguintes etapas:

1. Análise do fluxo do protótipo de alta fidelidade, a fim de compreender a navegação esperada do usuário e as principais telas envolvidas em cada funcionalidade;
2. Identificação dos atores participantes em cada cenário, principalmente passageiro, motorista e sistema;
3. Levantamento dos objetos e componentes envolvidos nas interações, como interface da aplicação, controladores, serviços, APIs e banco de dados;
4. Mapeamento das mensagens trocadas entre os participantes, respeitando a ordem cronológica das ações representadas nos fluxos do protótipo;
5. Construção dos diagramas de sequência na ferramenta Draw.io, utilizando a notação UML adequada para linhas de vida, mensagens, retornos e fragmentos condicionais quando necessário;
6. Revisão dos diagramas com base nos modelos estruturais do projeto, como os diagramas de classes e de componentes, para manter coerência entre a modelagem estática e a modelagem dinâmica;
7. Verificação final por meio de checklist, considerando critérios de consistência, completude, clareza e conformidade com a UML.

Dessa forma, a metodologia adotada permite que os diagramas de sequência sejam derivados de fluxos reais de uso da aplicação, mantendo rastreabilidade com o protótipo de alta fidelidade e apoiando a validação do comportamento esperado do sistema **Carona Amiga FCTE**.

## Sobre o Diagrama de Sequência

<a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-6">[6]</a>

Como apresentado na introdução, o diagrama de sequência é utilizado para representar, em ordem temporal, a interação entre atores, objetos e componentes durante a execução de um fluxo específico do sistema. No contexto do **Carona Amiga FCTE**, as linhas de vida são definidas a partir dos participantes identificados nos artefatos de modelagem, especialmente no diagrama de componentes, o que contribui para a coerência entre a estrutura do sistema e o comportamento descrito neste documento.

Na referência **O que é um diagrama de sequência UML?** <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-6">[6]</a>, os participantes são organizados horizontalmente e associados a linhas de vida verticais, enquanto as mensagens são representadas por setas que indicam chamadas, respostas e ativações ao longo do tempo. Esses elementos permitem descrever com maior clareza a comunicação entre passageiro, motorista e sistema, facilitando o entendimento dos fluxos modelados.

## Sobre o Diagrama de Sequência

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Cadastro de usuário</strong></summary>

**Cenário:**

A tabela 1 apresenta a estrutura de apoio para o detalhamento do diagrama de sequência de cadastro de usuário.

| Elemento do Diagrama de Sequência | Descrição na Sequência | Relação com Diagrama de Classes | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes |
| :-------------------------------- | :--------------------- | :------------------------------ | :--------------------------- | :---------------------------------- |
|                                   |                        |                                 |                              |                                     |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 1, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 1: Diagrama de Sequência - Cadastro de usuário
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Login</strong></summary>

**Cenário:**

A tabela 2 apresenta a estrutura de apoio para o detalhamento do diagrama de sequência de login.

| Elemento do Diagrama de Sequência | Descrição na Sequência | Relação com Diagrama de Classes | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes |
| :-------------------------------- | :--------------------- | :------------------------------ | :--------------------------- | :---------------------------------- |
|                                   |                        |                                 |                              |                                     |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 2, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 2: Diagrama de Sequência - Login
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Busca de caronas</strong></summary>

**Cenário:**

A tabela 3 apresenta a estrutura de apoio para o detalhamento do diagrama de sequência de busca de caronas.

| Elemento do Diagrama de Sequência | Descrição na Sequência | Relação com Diagrama de Classes | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes |
| :-------------------------------- | :--------------------- | :------------------------------ | :--------------------------- | :---------------------------------- |
|                                   |                        |                                 |                              |                                     |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 3, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 3: Diagrama de Sequência - Busca de caronas
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Solicitação de participação em carona</strong></summary>

**Cenário:**

A tabela 4 apresenta a estrutura de apoio para o detalhamento do diagrama de sequência de solicitação de participação em carona.

| Elemento do Diagrama de Sequência | Descrição na Sequência | Relação com Diagrama de Classes | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes |
| :-------------------------------- | :--------------------- | :------------------------------ | :--------------------------- | :---------------------------------- |
|                                   |                        |                                 |                              |                                     |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>
Com base na tabela 4, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 4: Diagrama de Sequência - Solicitação de participação em carona
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Publicação de carona</strong></summary>

**Cenário:**

A tabela 5 apresenta a estrutura de apoio para o detalhamento do diagrama de sequência de publicação de carona.

| Elemento do Diagrama de Sequência | Descrição na Sequência | Relação com Diagrama de Classes | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes |
| :-------------------------------- | :--------------------- | :------------------------------ | :--------------------------- | :---------------------------------- |
|                                   |                        |                                 |                              |                                     |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>

Com base na tabela 5, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 5: Diagrama de Sequência - Publicação de carona
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Confirmação de embarque</strong></summary>

**Cenário:**

Após a carona ser aceita, o passageiro chega ao ponto combinado e informa sua chegada pelo aplicativo. O sistema consulta os dados da carona, solicita a confirmação do motorista e, quando o embarque é confirmado, atualiza o status da viagem e informa o passageiro.

A tabela 6 apresenta, de forma simples, os elementos envolvidos no fluxo de confirmação de embarque.

Para manter a rastreabilidade com os requisitos elicitados na Entrega 01, foram usados apenas os requisitos que se relacionam com o fluxo de confirmação de embarque:

- [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu): Configurar pareamento de carona.
- [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Rastrear carona em tempo real.
- [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Configurar preferências de pareamento.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                      | Relação com Diagrama de Classes                              | Relação com Requisitos (RFs)                        | Relação com Diagrama de Componentes                  |
| :-------------------------------- | :-------------------------------------------------------------------------- | :----------------------------------------------------------- | :-------------------------------------------------- | :--------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                             |                                                              |                                                     |                                                      |
| `Passageiro` (Ator)               | Informa que chegou ao ponto de embarque e aguarda a confirmação.            | `Usuario` com papel de passageiro, associado à `Carona` por uma `Participacao` ou `Solicitacao`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Ator externo que interage com o componente `App CaronaAmiga`. |
| `App CaronaAmiga`                 | Recebe a ação do passageiro e exibe o resultado da confirmação.             | Interface que aciona operações sobre `Carona`, `Usuario` e `Participacao`. | [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Componente de interface que se comunica com o `Sistema de Caronas`. |
| `Sistema de Caronas`              | Consulta a carona, solicita a confirmação ao motorista e atualiza o status. | Serviço/controlador que manipula `Carona`, `Viagem`, `Usuario` e `Participacao`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff), [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Componente de negócio que coordena `App CaronaAmiga` e `Banco de Dados`. |
| `Banco de Dados`                  | Retorna os dados da carona e salva a confirmação do embarque.               | Persistência dos dados de `Carona`, `Usuario`, `Viagem` e `Participacao`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Componente de persistência acessado pelo `Sistema de Caronas`. |
| `Motorista` (Ator)                | Confirma que o passageiro embarcou.                                         | `Usuario` com papel de motorista, responsável pela `Carona` ou `Viagem`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff), [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Ator externo que recebe a solicitação pelo `App CaronaAmiga`. |
| **Mensagens / Interações Chave**  |                                                                             |                                                              |                                                     |                                                      |
| `1: informarChegada()`            | Passageiro informa que chegou ao ponto combinado.                           | Método associado à `Participacao` do passageiro em uma `Carona`. | [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do ator externo `Passageiro` com o componente `App CaronaAmiga`. |
| `2: solicitarConfirmacao()`       | App envia a solicitação de confirmação ao sistema.                          | Método de controle sobre `Carona` e `Participacao`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do `App CaronaAmiga` com o componente `Sistema de Caronas`. |
| `3: consultarCarona()`            | Sistema consulta os dados da carona.                                        | Consulta instâncias de `Carona`, `Usuario` e `Participacao`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do `Sistema de Caronas` com o componente `Banco de Dados`. |
| `5: pedirConfirmacao()`           | Sistema solicita ao motorista a confirmação do embarque.                    | Usa a relação entre `Motorista`, `Passageiro` e `Carona`. | [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu), [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do `Sistema de Caronas` com o ator externo `Motorista`. |
| `6: confirmarEmbarque()`          | Motorista confirma que o passageiro embarcou.                               | Atualiza o status da `Participacao` vinculada à `Carona`. | [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do ator externo `Motorista` com o `App CaronaAmiga`. |
| `8: atualizarStatus()`            | Sistema salva a confirmação do embarque.                                    | Atualiza o estado de `Participacao`, `Carona` ou `Viagem`. | [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff). | Comunicação do `Sistema de Caronas` com o componente `Banco de Dados`. |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>

Com base na tabela 6, abaixo será inserido o diagrama de sequência correspondente.

<div align="center">
    Figura 6: Diagrama de Sequência - Confirmação de embarque
    <br>
    <i>Inserir diagrama de sequência correspondente.</i>
    <br>
</div>

</details>
</div>

## Conclusão

O diagrama de sequência amplia a compreensão do comportamento do **Carona Amiga FCTE** ao organizar, de forma temporal, as interações entre usuários e componentes do sistema. Com a definição dos cenários futuros priorizados, a documentação passa a orientar com mais clareza a continuidade da modelagem dinâmica, mantendo coerência com os requisitos e com os demais artefatos do projeto.

---

## Referências bibliográficas

> <a id="referencias-bibliograficas-1">1.</a> APOSTILA UML. **Unified Modeling Language – Linguagem de Modelagem Unificada em Português**. Seção sobre diagrama de sequência. Disponibilizada pela professora. Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> IBM. **Diagramas de Sequência**. Disponível em: https://www.ibm.com/docs/pt-br/rsm/7.5.0?topic=uml-sequence-diagrams. Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> CARONA AMIGA FCTE. **Protótipo de Alta Fidelidade**. Disponível em: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo. Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-4">4.</a> UML Diagrams. **UML Sequence Diagrams Overview**. Disponível em: https://www.uml-diagrams.org/sequence-diagrams.html. Acesso em: 21 set. 2025.

> <a id="referencias-bibliograficas-5">5.</a> CREATELY. **Tutorial do Diagrama de Sequência: Guia completo com exemplos**. Disponível em: https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-sequencia/. Acesso em: 30 abr. 2025.

> <a id="referencias-bibliograficas-6">6.</a> LUCIDCHART. **O que é um diagrama de sequência UML?** Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml. Acesso em: 30 abr. 2025.

---

## Histórico de versão

| Versão | Data       | Descrição                                     | Autor(es)                                                   | Revisor(es)                                                 | Detalhes da Revisão |
| ------ | ---------- | --------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ------------------- |
| 1.0    | 21/04/2026 | Criação do artefato                           | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado   |
| 1.1    | 21/04/2026 | Adição da Introdução, objetivos e metodologia | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado   |
| 1.2    | 22/04/2026 | Adição do modelo do Diagrama de Sequência     | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Aguardando revisão  |
| 1.3    | 23/04/2026 | Adição do fluxo de confirmação de embarque    | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Aguardando revisão  |
