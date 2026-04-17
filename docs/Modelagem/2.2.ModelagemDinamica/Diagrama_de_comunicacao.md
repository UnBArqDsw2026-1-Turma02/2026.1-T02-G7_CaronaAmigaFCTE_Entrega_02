# Diagrama de Comunicação

# Introdução
Diagrama de Comunicação, ou Diagrama de Colaboração no UML 1.x, é um tipo de UML que foca na interação entre elementos, representados como _lifeline_ ("linha de vida" em tradução livre), utilizando mensagens sequenciadas de formato livre.
Os elementos mais importantes nessa diagramação são: _frame_, _lifeline_, _message_. [1](#referências-bibliográfias)

## Objetivos

O objetivo desse artefato é representar de forma estruturada e sequencial as principais comunicações entre elementos do sistema Carona Amiga, com intuito de facilitar o desenvolvimento posterior do projeto, provendo clareamento para ambiguidades entre relacionamentos.
 Sendo assim, as metas principais desse artefato são:

- Apresentar o Diagrama de Comunicação do web app Carona Amiga, destacando as principais comunicações entre elementos;

- Documentar os relacionamentos entre atores do sistema;

- Fornecer uma base sólida para o desenvolvimento e manutenção do sistema;

## Metodologia

### Material Suplementar

1.  <img src="https://store-images.s-microsoft.com/image/apps.1409.13851527096222888.2b60149a-04a5-4578-a6b2-d7b7377332d5.c22d8e97-4d44-4304-9bd2-55f9d29c0f82?h=210" width="25" height="25" align="center">  O **Diagrama de Comunicação** será desenvolvido utilizando a ferramenta [Draw.io](https://app.diagrams.net/), a qual permite a criação de diagramas UML de forma prática e visual.

2. Como base para a definição do Diagrama de Comunicação, serão utilizadas as informações coletadas na [Entrega 01 do Projeto](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01), a qual inclui:

- **Requisitos Funcionais:** para identificar as funcionalidades que o sistema deve oferecer e, consequentemente, as Comunicação necessárias para implementá-las. [Requisitos funcionais](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md#rf01);

- **Requisitos Não Funcionais:** para considerar aspectos como desempenho, segurança, usabilidade, etc., que podem influenciar a estrutura do sistema e as Comunicação envolvidas.
[Requisitos não funcionais](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md#rf01);

Informações adicionais, como [5W2H](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/5w2h.md), [Brainstorming](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/Brainstorm.md), [Benchmarking](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/Benchmarking.md) e [Personas](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/5-Iniciativas-Extras/Personas.md), também serão consideradas para garantir que o diagrama de Comunicação reflita adequadamente as necessidades do sistema.

- **Atores do sistema:** [Atores do sistema identificados no Rich Picture](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/1.3.RichPicture.md);

3. Será utilizado o [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md) construído na etapa de Modelagem Estática como suporte para desenvolvimento das comunicações.

### Construção

1. Será definido o _frame heading_, nomeando o elemento e o tipo de diagrama.

2. Serão definidas os objetos/partes do projeto;

3. Serão elencados os relacionamentos e suas ligações;

4. Serão anexadas as funções associadas a cada ligação e sua expressão de comunicação;

5. Será feita a verificação e validação conforme a lógica construída no [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md);

6. Por fim, será verificado de acordo com uma [tabela de verificação](Modelagem/2.6.VerificacaoDosDiagramas/VerificacaoDosDiagramas.md) baseada nos critérios sintáticos e semânticos da UML.

## Composição — Notação UML

| Elemento | Descrição Elemento | Composição | Explicação |
|---|:--:|---|---|
| **Frame** | Retângulo utilizado para **nomear** diagramas de comunicação, com o nome num compartimento no canto superior esquerdo. | ![Frame](/Modelagem/assets/communication-frame-long.png) |**_Frame_** "_Interaction"_ para **Diagrama de Comunicação** _BuyItem_ |
| **Frame** | Obs: Ambos reference à nomeações plausíveis para esse diagrama. | ![Frame](/Modelagem/assets/communication-frame-short.png) |**_Frame_** "_Sd"_ para **Diagrama de Comunicação** _BuyItem_ |
| **Lifeline** | Representa um **participante individual** na interação, pode-se entender como uma relação 1 para 1. | ![Lifeline](/Modelagem/assets/communication-lifeline-named.png) | _Lifeline_ anônimo da classe _User_ |
|  | | ![Lifeline](/Modelagem/assets/communication-lifeline-no-name.png)  | **_Lifeline_** _"data"_ da classe _Stock_ |
|  | | ![Lifeline](/Modelagem/assets/communication-lifeline-selector.png)  | **_Lifeline_** _"x"_ da classe _X_ selecionado com *seletor* [k] |
| **Message** | Linha com sequência de expressão e uma seta acima, indicando a direção da comunicação. |![Message](/Modelagem/assets/communication-message.png) | Instância da classe **_A_ envia mensagem _remove()_ para** a instância de **_B_ se _s1_ for igual a _s2_**. |
| **Message** | |![Message](/Modelagem/assets/communication-message-sequence.png) | Instância de **_A_ envia mensagem _draw()_ para** a instância de **_B_**, depois **_B_ envia _paint()_ para C**. |
| **Message** | |![Message](/Modelagem/assets/communication-message-concurrent.png) | Instância de **_A_ envia mensagem _draw()_ para** a instância de **_B_** e instância de **C**, **concomitantemente**. |
| **Message** | |![Message](/Modelagem/assets/communication-message-guard.png) | Instância da classe **_A_ enviará mensagem _draw()_ para** a instância de **_C_ se _x_ for maior que _y_**. |
| **Message** | |![Message](/Modelagem/assets/communication-message-loop-sequence.png) | Instância da classe **_A_ enviará mensagem _search()_ para** a instância de **_B_ _n_ vezes, uma a uma**. |
| **Message** | |![Message](/Modelagem/assets/communication-message-loop-concurrent.png) | Instância da classe **_A_ enviará _n_ mensagens _search()_ concomitantemente para** a instância de **_B_**. |

## Diagrama de Comunicação


<div align="center">
              Figura 1: Diagrama de Comunicação.

![Diagrama de Comunicação](../assets/diagrama_de_comunicacao.png)


<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS),  [Luiza da Silva Pugas](https://github.com/luizaxx) e [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), 2026.</p></font>
</div>

## Conclusão

A elaboração do Diagrama de Colaboração para o projeto **Carona Amiga** possibilitou a representação de forma estruturada das interações entre as partes do projeto, usando mensagens de forma livre.

## Referências Bibliográfias

> 1. https://www.uml-diagrams.org/communication-diagrams.html
> 2. Materiasi de Aula, DSW-Modelagem - Comunicacao

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 17/04/2026 | Criação do documento | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [Luiza da Silva Pugas](https://github.com/luizaxx) e [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato revisado |