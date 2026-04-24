# Diagrama de Atividades

## Introdução

O Diagrama de Atividades é um diagrama comportamental da UML (Unified Modeling Language) que descreve o fluxo de controle ou o fluxo de dados de um sistema, detalhando a sequência lógica de passos, decisões e condições de um processo de negócio ou algoritmo. Diferente de outros diagramas que focam em quem faz, o foco é no o que acontece e em qual ordem.

Neste artefato, utilizamos Swimlanes (raias) para organizar as responsabilidades e fluxos principais do sistema Carona Amiga, permitindo visualizar processos complexos como o login, cadastro, solicitar e pedir caronas e a avaliação dos usuários.

---

## Objetivos

Este artefato tem como objetivo mapear os fluxos operacionais do web app **Carona Amiga**, garantindo que a lógica de negócio esteja clara. Sendo assim, busca-se:

- Apresentar o Diagrama de Atividades, destacando o fluxo de trabalho desde o acesso inicial até a conclusão de uma viagem;

- Documentar os pontos de decisão e caminhos alternativos do sistema;

- Identificar as principais funcionalidades (Login, Cadastro, Oferta, Pedido e Avaliação).

---

## Metodologia

O diagrama foi elaborado utilizando a ferramenta Draw.io. Também foram utilizados os requisitos elicitados na Entrega 01 do Projeto e as necessidades de interação do usuário final identificadas em personas e histórias de usuário.

Principais artefatos consultados:

- Backlog do Produto (Requisitos Funcionais);

- Personas e Cenários de Uso.

O processo adotado foi:

1. Divisão do sistema em 5 processos principais (Raias);

2. Mapeamento das ações sequenciais para cada processo;

3. Identificação de condições lógicas (ex: "Dados verificados?" ou "Pedido aceito?");

4. Revisão da sintaxe UML;

5. Validação da consistência lógica entre os fluxos.

---

## Construção

O diagrama foi construído seguindo as seguintes etapas:

1. Definição das Raias (Swimlanes): Organização vertical por domínio de funcionalidade (Login, Cadastro, Oferecer Carona, Pedir Carona e Avaliação).

2. Identificação de Gatilhos: Definição do nó inicial para cada processo.

3. Mapeamento de Ações: Inclusão de retângulos arredondados para representar as atividades executadas pelo sistema ou usuário.

4. Inserção de Lógica de Desvio: Uso de losangos para decisões que alteram o rumo do fluxo.

5. Finalização: Definição dos estados finais que indicam o encerramento da atividade.

---

## Composição — Notação UML

<font size="3"><p style="text-align: center">Tabela 1: Legenda do Elementos</p></font>

| Elemento | Composição | Símbolo | Explicação |
|---|:--:|---|---|
| **Nó Inicial**  | ● | Círculo Preto | Simboliza o início da atividade. |
| **Atividade**  | ▭ | Retângulo Arredondado | Ação em que o usuário ou software realiza uma determinada tarefa. |
| **Fluxo de Controle** | → | Seta Direcional | Conectores que mostram o fluxo entre as etapas no diagrama. |
| **Decisão**  | ◆ | Losango | Indica um ponto onde o fluxo pode seguir caminhos diferentes com base em uma condição. |
| **Swimlane (Raia)**  | — | Colunas Verticais | Organiza as atividades por categoria, ator ou funcionalidade. |
| **Nó Final** | ◎ | Círculo com borda | Indica o encerramento do fluxo de uma atividade específica. |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Diagrama de Atividades

<div align="center">
Figura 1: Diagrama de Atividades.

![Diagrama de Atividades](https://i.postimg.cc/zvGLRv5X/Diagrama-de-Atividades-drawio.png)

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>
</div>

---

## Conclusão

A construção do Diagrama de Atividades permitiu uma visão muito funcional dos processos do **Carona Amiga**. Através dele, foi possível identificar situações lógicas e garantir que todas as condições de erro (como dados inválidos no cadastro) tivessem um fluxo de retorno apropriado. Este artefato servirá como guia para a implementação das rotas e controladores do backend, assegurando que o comportamento do software reflita os requisitos de negócio.

---

## Referências

> Lucidchart. _O que é um diagrama de atividades UML?_. Disponível em: <https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-atividades-uml>.

> UML Diagrams. _UML activity diagrams overview_. Disponível em: https://www.uml-diagrams.org/activity-diagrams.html.

> SERRANO, Milene. _Slides - Diagrama de Atividades UML_. Disponível em: https://aprender3.unb.br/pluginfile.php/3178534/mod_page/content/1/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Modelagem%20UML%20Din%C3%A2mica%20-%20Profa.%20Milene.pdf.

---

## Histórico de Versões

| Versão | Data | Descrição | Autor | Revisor |
| :----: | :--: | --------- | ------ | ------ |
| 1.0 | 22/04/2026 | Criação do documento | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) |  [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) e [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) |
| 1.1 | 23/04/2026 | Adição de referências e ajustes no documento | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) |  [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) |
|1.2  | 23/04/2026 | Correção do link da imagem do diagrama e ajustes no documento | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) |
