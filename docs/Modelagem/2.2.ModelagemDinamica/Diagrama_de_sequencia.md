# Diagrama de Sequência

## Introdução

O diagrama de sequência é um dos principais artefatos da UML utilizados para representar o comportamento dinâmico de um sistema, evidenciando a troca de mensagens entre seus elementos ao longo do tempo. De acordo com a Apostila UML <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-1">[1]</a>, esse tipo de diagrama descreve, de forma visual e cronológica, como ocorre a interação entre atores e objetos envolvidos na execução de uma funcionalidade específica.

A estrutura de um diagrama de sequência é organizada em dois eixos principais: o eixo vertical, que representa o tempo (de cima para baixo), e o eixo horizontal, que apresenta os participantes da interação, cada um com sua respectiva linha de vida. As mensagens trocadas entre esses elementos são representadas por setas, permitindo visualizar com clareza a ordem das operações e a comunicação entre os componentes do sistema, conforme descrito pela Creately <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-4">[4]</a>.

No contexto do projeto **Carona Amiga FCTE**, os diagramas de sequência são utilizados para detalhar as interações entre os usuários, especialmente passageiros e motoristas — e os componentes internos da aplicação, como interface, APIs, serviços e banco de dados. Esses diagramas complementam os modelos estruturais previamente desenvolvidos, como os diagramas de classes e de componentes, garantindo consistência entre a arquitetura do sistema e seu comportamento em tempo de execução.

Dessa forma, a modelagem por meio de diagramas de sequência contribui para o entendimento dos fluxos principais da aplicação, como cadastro, autenticação, busca de caronas, solicitação de participação e gerenciamento de viagens. Além disso, auxilia na identificação de responsabilidades, na validação dos requisitos e no suporte às etapas de implementação e manutenção do sistema.

Tomando como base a legenda já elaborada para o projeto e as convenções da UML descritas na bibliografia adotada <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-1">[1]</a> <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-4">[4]</a>, a leitura dos diagramas considera elementos como participante ou objeto, linha de vida, mensagens síncronas e assíncronas, resposta ou retorno e autochamada. Essa padronização fortalece a rastreabilidade entre a fundamentação teórica, a representação visual utilizada pela equipe e os fluxos modelados para o **Carona Amiga FCTE**.

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

A elaboração dos diagramas de sequência do **Carona Amiga FCTE** seguirá uma abordagem iterativa, com base nos artefatos previamente construídos pela equipe e nos fluxos definidos no protótipo de alta fidelidade da aplicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>. A partir desses fluxos, o comportamento do sistema será observado sob a perspectiva temporal das interações, permitindo identificar a ordem das mensagens trocadas entre os atores, a interface, os serviços internos e a persistência dos dados.

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

Como apresentado na introdução, o diagrama de sequência é utilizado para representar, em ordem temporal, a interação entre atores, objetos e componentes durante a execução de um fluxo específico do sistema. No contexto do **Carona Amiga FCTE**, as linhas de vida são definidas a partir dos participantes identificados nos artefatos de modelagem, especialmente no diagrama de componentes, o que contribui para a coerência entre a estrutura do sistema e o comportamento descrito neste documento.

Na referência **O que é um diagrama de sequência UML?** <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-5">[5]</a>, os participantes são organizados horizontalmente e associados a linhas de vida verticais, enquanto as mensagens são representadas por setas que indicam chamadas, respostas e ativações ao longo do tempo. Esses elementos permitem descrever com maior clareza a comunicação entre passageiro, motorista e sistema, facilitando o entendimento dos fluxos modelados.

[RFU01]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu
[RFU02]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu
[RFM01]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-motiva%c3%a7%c3%a3o-do-usu%c3%a1rio-rfm
[RFM02]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-motiva%c3%a7%c3%a3o-do-usu%c3%a1rio-rfm
[RFS01]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-seguran%c3%a7a-do-usu%c3%a1rio-rfs
[RFS02]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-seguran%c3%a7a-do-usu%c3%a1rio-rfs
[RFS03]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-seguran%c3%a7a-do-usu%c3%a1rio-rfs
[RFS04]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-seguran%c3%a7a-do-usu%c3%a1rio-rfs
[RFF01]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff
[RFF02]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff
[RFF03]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff
[RFF06]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff
[RFF07]: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff

## Sobre o Diagrama de Sequência

<div style="margin-left: 20px;">
<details style="margin-bottom: 20px;">
  <summary style="font-size: 1.1rem;"><strong>Fluxo: Cadastro de usuário</strong></summary>

**Cenário:**

O usuário acessa a tela de cadastro, informa seus dados institucionais e, quando aplicável, registra dados de veículo e preferências iniciais. O sistema valida o e-mail institucional, cria o perfil e armazena as informações necessárias para uso posterior da plataforma.

A tabela 1 apresenta, de forma simples, os elementos envolvidos no fluxo de cadastro de usuário.

Seguindo os requisitos elicitados na Entrega 01, foram usados apenas os requisitos relacionados ao fluxo de cadastro de usuário:

- [`RFU01`][RFU01]: Informar disponibilidade de CNH e veículo.
- [`RFU02`][RFU02]: Configurar pareamento de carona.
- [`RFS01`][RFS01]: Exibir perfil com foto.
- [`RFS02`][RFS02]: Validar matrícula institucional.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                 | Relação com Diagrama de Classes                                                                                   | Relação com Requisitos (RFs)                          | Relação com Diagrama de Componentes                                                 |
| :-------------------------------- | :--------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------- | :---------------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                        |                                                                                                                   |                                                       |                                                                                     |
| `Usuário` (Ator)                  | Preenche os dados de cadastro e informa se possui CNH ou veículo.      | Instância de `Usuario`; pode se especializar em `Motorista` ou `Passageiro`.                                      | [`RFU01`][RFU01], [`RFS02`][RFS02].                   | Relaciona-se aos componentes `:Motorista` e `:Passageiro` do subsistema `Usuários`. |
| `:Cadastro`                       | Recebe os dados do formulário de criação de conta.                     | Aciona `Usuario.cadastrar()` e registra `emailInstitucional`, `senhaHash`, `nome`, `fotoPerfil` e `preferencias`. | [`RFS01`][RFS01], [`RFS02`][RFS02].                   | Componente do subsistema `autentificação`, ligado à `Authentication interface`.     |
| `:Auth Service`                   | Valida o vínculo institucional e autoriza a criação do usuário.        | Apoia a criação de `Usuario` e valida `emailInstitucional`.                                                       | [`RFS02`][RFS02].                                     | Componente do subsistema `Backend` que provê `Authentication interface`.            |
| `:UserService`                    | Registra dados de perfil e preferências iniciais.                      | Manipula `Usuario`, `PreferenciaPareamento` e, quando necessário, `Veiculo`.                                      | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS01`][RFS01]. | Componente do `Backend` que provê `Passenger profile interface`.                    |
| `:Banco de dados Carona`          | Armazena usuário, perfil, preferências e dados de veículo.             | Persiste `Usuario`, `PreferenciaPareamento` e `Veiculo`.                                                          | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS02`][RFS02]. | Componente de persistência do subsistema `GerenciamentoCaronas`.                    |
| **Mensagens / Interações Chave**  |                                                                        |                                                                                                                   |                                                       |                                                                                     |
| `1: preencherCadastro()`          | Usuário informa dados pessoais, institucionais e opcionais de veículo. | Preenche atributos de `Usuario` e, se for motorista, de `Veiculo`.                                                | [`RFU01`][RFU01], [`RFS01`][RFS01], [`RFS02`][RFS02]. | Comunicação do ator com `:Cadastro`.                                                |
| `2: cadastrar()`                  | Cadastro solicita criação do usuário.                                  | Método `Usuario.cadastrar()`.                                                                                     | [`RFS02`][RFS02].                                     | `:Cadastro` consome `Authentication interface` de `:Auth Service`.                  |
| `3: validarEmailInstitucional()`  | Auth Service valida o e-mail ou matrícula institucional.               | Usa `Usuario.emailInstitucional`.                                                                                 | [`RFS02`][RFS02].                                     | Processamento interno do `:Auth Service`.                                           |
| `4: atualizarPreferencias()`      | Sistema registra preferências iniciais de pareamento.                  | Método `PreferenciaPareamento.atualizar()`.                                                                       | [`RFU02`][RFU02].                                     | `:UserService` expõe dados via `Passenger profile interface`.                       |
| `5: validarDocumentacao()`        | Quando houver veículo, a documentação é validada.                      | Método `Veiculo.validarDocumentacao(String Placa)`.                                                               | [`RFU01`][RFU01].                                     | `:UserService` persiste os dados em `:Banco de dados Carona`.                       |
| `6: confirmarCadastro()`          | Cadastro confirma a criação da conta para o usuário.                   | Retorno da criação de `Usuario`.                                                                                  | [`RFS02`][RFS02].                                     | `:Cadastro` retorna resultado ao componente de usuário.                             |

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

O usuário informa suas credenciais de acesso. O sistema valida os dados com o serviço de autenticação, recupera o perfil associado e libera o acesso ao aplicativo conforme o tipo de usuário.

A tabela 2 apresenta, de forma simples, os elementos envolvidos no fluxo de login.

Seguindo os requisitos elicitados na Entrega 01, foi usado apenas o requisito relacionado ao controle de vínculo institucional no acesso:

- [`RFS02`][RFS02]: Validar matrícula institucional.

| Elemento do Diagrama de Sequência | Descrição na Sequência                               | Relação com Diagrama de Classes                                          | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes                                                 |
| :-------------------------------- | :--------------------------------------------------- | :----------------------------------------------------------------------- | :--------------------------- | :---------------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                      |                                                                          |                              |                                                                                     |
| `Usuário` (Ator)                  | Informa e-mail institucional e senha.                | Instância de `Usuario`, `Motorista` ou `Passageiro`.                     | [`RFS02`][RFS02].            | Relaciona-se aos componentes `:Motorista` e `:Passageiro` no subsistema `Usuários`. |
| `:Login`                          | Recebe as credenciais e inicia a autenticação.       | Aciona `Usuario.login()` usando `emailInstitucional` e `senhaHash`.      | [`RFS02`][RFS02].            | Componente do subsistema `autentificação`.                                          |
| `:Auth Service`                   | Valida credenciais e vínculo institucional.          | Verifica dados de `Usuario`.                                             | [`RFS02`][RFS02].            | Componente do `Backend` que provê `Authentication interface` em OAuth2.             |
| `:UserService`                    | Recupera dados do perfil para entrada no aplicativo. | Consulta `Usuario`, `Motorista`, `Passageiro` e `PreferenciaPareamento`. | [`RFS02`][RFS02].            | Componente que provê `Passenger profile interface`.                                 |
| **Mensagens / Interações Chave**  |                                                      |                                                                          |                              |                                                                                     |
| `1: informarCredenciais()`        | Usuário informa e-mail e senha.                      | Usa `Usuario.emailInstitucional` e `Usuario.senhaHash`.                  | [`RFS02`][RFS02].            | Comunicação do ator com `:Login`.                                                   |
| `2: login()`                      | Login solicita autenticação.                         | Método `Usuario.login(): Boolean`.                                       | [`RFS02`][RFS02].            | `:Login` consome `Authentication interface` de `:Auth Service`.                     |
| `3: validarUsuario()`             | Auth Service valida o usuário cadastrado.            | Verifica a instância de `Usuario`.                                       | [`RFS02`][RFS02].            | Processamento interno do `:Auth Service`.                                           |
| `4: carregarPerfil()`             | Sistema recupera dados do perfil autenticado.        | Usa `Usuario.getHistorico()` e dados de `Motorista` ou `Passageiro`.     | [`RFS02`][RFS02].            | `:UserService` provê dados pela `Passenger profile interface`.                      |
| `5: liberarAcesso()`              | Login libera o acesso ao aplicativo.                 | Retorno positivo de `Usuario.login()`.                                   | [`RFS02`][RFS02].            | Retorno para `:App Motorista` ou `:App Passageiro` via `Authentication interface`.  |

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

O passageiro informa critérios de busca, como origem, destino, horário, escopo e preferências de pareamento. O sistema consulta as caronas disponíveis, aplica filtros, calcula informações de rota e exibe opções compatíveis.

A tabela 3 apresenta, de forma simples, os elementos envolvidos no fluxo de busca de caronas.

Seguindo os requisitos elicitados na Entrega 01, foram usados apenas os requisitos relacionados ao fluxo de busca de caronas:

- [`RFU02`][RFU02]: Configurar pareamento de carona.
- [`RFM01`][RFM01]: Selecionar contexto de uso da carona.
- [`RFM02`][RFM02]: Exibir estimativa de custo e duração.
- [`RFS01`][RFS01]: Exibir perfil com foto.
- [`RFS03`][RFS03]: Permitir avaliação de usuários.
- [`RFS04`][RFS04]: Exibir amigos em comum.
- [`RFF02`][RFF02]: Dividir custos da viagem.
- [`RFF06`][RFF06]: Configurar preferências de pareamento.
- [`RFF07`][RFF07]: Selecionar escopo de caronas.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                | Relação com Diagrama de Classes                                                                                                    | Relação com Requisitos (RFs)                                            | Relação com Diagrama de Componentes                                           |
| :-------------------------------- | :-------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                       |                                                                                                                                    |                                                                         |                                                                               |
| `Passageiro` (Ator)               | Informa filtros e consulta caronas disponíveis.                       | Especialização de `Usuario` com métodos `getPreferencias()` e `FavoritarMotorista()`.                                              | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Ator externo representado pelo componente `:Passageiro`.                      |
| `:App Passageiro`                 | Exibe filtros, resultados e detalhes da carona.                       | Interface que apresenta dados de `Carona`, `Motorista`, `Avaliacao`, `Rota` e `Localizacao`.                                       | [`RFM02`][RFM02], [`RFS01`][RFS01], [`RFS03`][RFS03], [`RFS04`][RFS04]. | Componente do subsistema `client` que consome `Ride management interface`.    |
| `:Carona`                         | Exibe dados resumidos e detalhados da corrida.                        | Relaciona-se à classe `Carona` e seus atributos `origem`, `destino`, `horarioPartida`, `vagasDisponiveis`, `precoBase` e `status`. | [`RFM01`][RFM01], [`RFM02`][RFM02], [`RFF02`][RFF02].                   | Componente do subsistema `interface` que consome `Ride management interface`. |
| `:Ride API`                       | Processa a busca e solicita dados ao backend.                         | Coordena consulta de `Carona`, `PreferenciaPareamento`, `Rota` e `Localizacao`.                                                    | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Componente do `Backend` que provê `Ride management interface`.                |
| `:Location Service`               | Calcula dados de rota e estimativas.                                  | Usa `Rota.calcularRota(Array Localizacao[])`, `Rota.calcularTempoEstimadoMin(Array pontos)` e `Localização.getCoordenadas()`.      | [`RFM02`][RFM02].                                                       | Componente do `Backend` que provê `Ride tracking interface`.                  |
| `:Banco de dados Carona`          | Retorna caronas, motoristas, avaliações e dados de rota.              | Persiste `Carona`, `Motorista`, `Avaliacao`, `Rota` e `Localização`.                                                               | [`RFS03`][RFS03], [`RFF07`][RFF07].                                     | Componente do subsistema `GerenciamentoCaronas`.                              |
| **Mensagens / Interações Chave**  |                                                                       |                                                                                                                                    |                                                                         |                                                                               |
| `1: informarFiltros()`            | Passageiro informa origem, destino, horário, contexto e preferências. | Usa `Passageiro.getPreferencias()` e `PreferenciaPareamento.atualizar()`.                                                          | [`RFU02`][RFU02], [`RFM01`][RFM01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | Comunicação do `Passageiro` com `:App Passageiro`.                            |
| `2: buscarCaronas()`              | App solicita a lista de caronas disponíveis.                          | Consulta objetos `Carona` com `status: StatusCarona`.                                                                              | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | `:App Passageiro` consome `Ride management interface` de `:Ride API`.         |
| `3: aplicarFiltro()`              | Sistema filtra caronas compatíveis.                                   | Método `PreferenciaPareamento.aplicarFiltro(Carona[*])`.                                                                           | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Processamento da `:Ride API` com apoio do `:API Gateway`.                     |
| `4: calcularEstimativas()`        | Sistema calcula rota, tempo, distância e custo aproximado.            | Métodos de `Rota` e atributo `Carona.precoBase`.                                                                                   | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Comunicação da `:Ride API` com `:Location Service`.                           |
| `5: consultarPerfilMotorista()`   | Sistema recupera foto, avaliação e sinais de confiança.               | Consulta `Motorista`, `Usuario.fotoPerfil`, `Avaliacao.getMedia()` e relações sociais.                                             | [`RFS01`][RFS01], [`RFS03`][RFS03], [`RFS04`][RFS04].                   | `:UserService` provê dados pela `Passenger profile interface`.                |
| `6: exibirOpcoes()`               | App apresenta as caronas compatíveis ao passageiro.                   | Exibe dados de `Carona`, `Motorista`, `Rota` e `Avaliacao`.                                                                        | [`RFM02`][RFM02], [`RFS01`][RFS01], [`RFS03`][RFS03].                   | Retorno da `Ride management interface` para `:App Passageiro`.                |

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

O passageiro seleciona uma carona disponível, confere as principais informações e solicita participação. O sistema valida a disponibilidade da carona e as regras de pareamento, registra a solicitação e notifica o motorista para análise.

A tabela 4 apresenta, de forma simples, os elementos envolvidos no fluxo de solicitação de participação em carona.

Seguindo os requisitos elicitados na Entrega 01, foram usados apenas os requisitos relacionados ao fluxo de solicitação de participação em carona:

- [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu): Configurar pareamento de carona.
- [`RFM02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-motiva%c3%a7%c3%a3o-do-usu%c3%a1rio-rfm): Exibir estimativa de custo e duração.
- [`RFF01`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Agendar caronas.
- [`RFF02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Dividir custos da viagem.
- [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Configurar preferências de pareamento.
- [`RFF07`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Selecionar escopo de caronas.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                     | Relação com Diagrama de Classes                                                                                                              | Relação com Requisitos (RFs)                                            | Relação com Diagrama de Componentes                                                             |
| :-------------------------------- | :------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                            |                                                                                                                                              |                                                                         |                                                                                                 |
| `Passageiro` (Ator)               | Escolhe uma carona e solicita participação.                                | Classe `Passageiro`, especialização de `Usuario`, usando `solicitarCarona()` e `getPreferencias()`.                                          | [`RFU02`][RFU02], [`RFM02`][RFM02], [`RFF01`][RFF01].                   | Ator externo representado pelo componente `:Passageiro`.                                        |
| `:App Passageiro`                 | Exibe detalhes da carona e envia a solicitação.                            | Apresenta dados de `Carona`, `Motorista`, `Avaliacao` e `PreferenciaPareamento`.                                                             | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Componente do subsistema `client`; consome `Ride management interface`.                         |
| `:Ride API / :API Gateway`        | Valida disponibilidade, preferências e regras antes de registrar o pedido. | Coordena `Carona.vagasDisponiveis`, `Carona.passageiros`, `Passageiro.solicitarCarona()` e `PreferenciaPareamento.aplicarFiltro(Carona[*])`. | [`RFU02`][RFU02], [`RFF01`][RFF01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | `:Ride API` provê `Ride management interface`; `:API Gateway` roteia a chamada.                 |
| `:Banco de dados Carona`          | Armazena o vínculo do passageiro com a carona solicitada.                  | Persiste atualização em `Carona.passageiros: Array[Passageiro]` e `vagasDisponiveis`.                                                        | [`RFU02`][RFU02], [`RFF01`][RFF01].                                     | Componente de persistência do subsistema `GerenciamentoCaronas`.                                |
| `Motorista` (Ator)                | Recebe a notificação de nova solicitação para sua carona.                  | Classe `Motorista`, responsável pela `Carona`, com método `aceitarPassageiro()`.                                                             | [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Ator externo representado pelo componente `:Motorista`, notificado via `:Notification Service`. |
| **Mensagens / Interações Chave**  |                                                                            |                                                                                                                                              |                                                                         |                                                                                                 |
| `1: selecionarCarona()`           | Passageiro seleciona a carona desejada.                                    | Consulta uma instância de `Carona` associada a `Motorista`.                                                                                  | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Comunicação do `Passageiro` com `:App Passageiro`.                                              |
| `2: solicitarCarona()`            | App envia o pedido de participação ao sistema.                             | Método `Passageiro.solicitarCarona()`.                                                                                                       | [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | `:App Passageiro` consome `Ride management interface` de `:Ride API`.                           |
| `3: aplicarFiltro()`              | Sistema verifica vagas, horário, escopo e preferências.                    | Método `PreferenciaPareamento.aplicarFiltro(Carona[*])`; consulta `Carona.vagasDisponiveis`.                                                 | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Processamento em `:Ride API` com roteamento pelo `:API Gateway`.                                |
| `4: registrarPassageiro()`        | Sistema registra a solicitação na carona.                                  | Atualiza `Carona.passageiros` e `vagasDisponiveis`.                                                                                          | [`RFF01`][RFF01].                                                       | Comunicação do `:Ride API` com `:Banco de dados Carona`.                                        |
| `5: dispararNotificacao()`        | Sistema informa ao motorista que há uma nova solicitação.                  | Método `Notificacao.disparar()`, com destinatário `Motorista`.                                                                               | [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | `:Notification Service` envia evento para `:Notificação de Carona` e `:App Motorista`.          |
| `6: exibirSolicitacaoEnviada()`   | App confirma ao passageiro que a solicitação foi enviada.                  | Retorno da execução de `Passageiro.solicitarCarona()`.                                                                                       | [`RFF01`][RFF01].                                                       | Retorno da `Ride management interface` para `:App Passageiro`.                                  |

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

O motorista acessa o aplicativo, informa os dados da carona, define rota, horário, vagas e preferências de pareamento. O sistema valida as informações, registra a carona no banco de dados e confirma a publicação para que ela fique disponível aos passageiros compatíveis.

A tabela 5 apresenta, de forma simples, os elementos envolvidos no fluxo de publicação de carona.

Seguindo os requisitos elicitados na Entrega 01, foram usados apenas os requisitos relacionados ao fluxo de publicação de carona:

- [`RFU01`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu): Informar disponibilidade de CNH e veículo.
- [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu): Configurar pareamento de carona.
- [`RFM01`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-%c3%a0-motiva%c3%a7%c3%a3o-do-usu%c3%a1rio-rfm): Selecionar contexto de uso da carona.
- [`RFF01`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Agendar caronas.
- [`RFF02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Dividir custos da viagem.
- [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Configurar preferências de pareamento.
- [`RFF07`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Selecionar escopo de caronas.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                               | Relação com Diagrama de Classes                                                                                                                            | Relação com Requisitos (RFs)                                                              | Relação com Diagrama de Componentes                                              |
| :-------------------------------- | :------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                      |                                                                                                                                                            |                                                                                           |                                                                                  |
| `Motorista` (Ator)                | Informa os dados da carona que deseja publicar.                      | Classe `Motorista`, especialização de `Usuario`, associada a `Veiculo` e `Carona`.                                                                         | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Ator externo representado pelo componente `:Motorista`.                          |
| `:App Motorista`                  | Exibe formulário de publicação e envia os dados preenchidos.         | Interface que aciona `Motorista.publicarCarona()` e exibe dados de `Carona`, `Veiculo` e `Rota`.                                                           | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Componente do subsistema `client` que consome `Ride management interface`.       |
| `:Ride API / :API Gateway`        | Valida os dados, aplica preferências e registra a nova carona.       | Coordena `Motorista.validarCarona()`, `Carona.publicar()`, `Veiculo.validarDocumentacao(String Placa)` e `PreferenciaPareamento.aplicarFiltro(Carona[*])`. | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF01`][RFF01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | `:Ride API` provê `Ride management interface`; `:API Gateway` roteia a operação. |
| `:Location Service`               | Apoia cálculo de rota, tempo e distância da carona.                  | Usa `Rota.calcularRota(Array Localizacao[])`, `Rota.calcularTempoEstimadoMin(Array pontos)` e `Localização.getCoordenadas()`.                              | [`RFM01`][RFM01], [`RFM02`][RFM02].                                                       | Componente do `Backend` que provê `Ride tracking interface`.                     |
| `:Banco de dados Carona`          | Armazena a carona publicada e seus dados principais.                 | Persiste `Carona`, `Motorista`, `Veiculo`, `Rota`, `Localização` e `StatusCarona`.                                                                         | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Componente de persistência do subsistema `GerenciamentoCaronas`.                 |
| **Mensagens / Interações Chave**  |                                                                      |                                                                                                                                                            |                                                                                           |                                                                                  |
| `1: abrirPublicacao()`            | Motorista acessa a opção de publicar carona.                         | Operação iniciada por `Motorista`.                                                                                                                         | [`RFU01`][RFU01].                                                                         | Comunicação do ator `Motorista` com `:App Motorista`.                            |
| `2: preencherDadosCarona()`       | Motorista informa origem, destino, horário, vagas, contexto e custo. | Preenche atributos de `Carona`: `origem`, `destino`, `horarioPartida`, `vagasDisponiveis` e `precoBase`.                                                   | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Interação do `Motorista` com `:App Motorista`.                                   |
| `3: publicarCarona()`             | App envia os dados da nova carona ao sistema.                        | Método `Motorista.publicarCarona()` e `Carona.publicar()`.                                                                                                 | [`RFF01`][RFF01], [`RFF02`][RFF02].                                                       | `:App Motorista` consome `Ride management interface` de `:Ride API`.             |
| `4: validarCarona()`              | Sistema verifica motorista, veículo, rota, horário e preferências.   | Métodos `Motorista.validarCarona()`, `Veiculo.validarDocumentacao(String Placa)` e `PreferenciaPareamento.aplicarFiltro(Carona[*])`.                       | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Processamento em `:Ride API`, com apoio de `:Location Service`.                  |
| `5: salvarCarona()`               | Sistema registra a carona publicada.                                 | Persiste `Carona.status: StatusCarona`, `motorista: Motorista` e `passageiros: Array[Passageiro]`.                                                         | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Comunicação do `:Ride API` com `:Banco de dados Carona`.                         |
| `6: confirmarPublicacao()`        | App informa que a carona foi publicada com sucesso.                  | Retorno da execução de `Carona.publicar()`.                                                                                                                | [`RFF01`][RFF01].                                                                         | Retorno da `Ride management interface` para `:App Motorista`.                    |

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

Seguindo os requisitos elicitados na Entrega 01, foram usados apenas os requisitos relacionados ao fluxo de confirmação de embarque:

- [`RFU02`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-referentes-ao-perfil-de-usu%c3%a1rio-rfu): Configurar pareamento de carona.
- [`RFF03`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Rastrear carona em tempo real.
- [`RFF06`](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario?id=requisitos-elicitados-de-funcionalidades-desejadas-rff): Configurar preferências de pareamento.

| Elemento do Diagrama de Sequência | Descrição na Sequência                                    | Relação com Diagrama de Classes                                                                           | Relação com Requisitos (RFs)                          | Relação com Diagrama de Componentes                                                    |
| :-------------------------------- | :-------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                           |                                                                                                           |                                                       |                                                                                        |
| `Passageiro` (Ator)               | Informa chegada ao ponto de embarque e aguarda validação. | Classe `Passageiro`, especialização de `Usuario`, vinculada à `Carona.passageiros`.                       | [`RFU02`][RFU02], [`RFF03`][RFF03].                   | Ator externo representado pelo componente `:Passageiro`.                               |
| `:App Passageiro`                 | Envia a chegada e exibe o resultado da confirmação.       | Interface que apresenta dados de `Carona`, `ValidacaoEmbarque` e `StatusCarona`.                          | [`RFF03`][RFF03].                                     | Componente do subsistema `client`; consome `Ride management interface`.                |
| `:Ride API / :API Gateway`        | Consulta a carona, gera/valida código e atualiza status.  | Coordena `Carona.confirmarEmbarque()`, `ValidacaoEmbarque.gerarCodigo()` e `ValidacaoEmbarque.validar()`. | [`RFU02`][RFU02], [`RFF03`][RFF03], [`RFF06`][RFF06]. | `:Ride API` provê `Ride management interface`; `:API Gateway` roteia a operação.       |
| `:Banco de dados Carona`          | Retorna dados da carona e salva a validação do embarque.  | Persiste `Carona`, `ValidacaoEmbarque`, `StatusCarona` e `HistoricoViagem`.                               | [`RFU02`][RFU02], [`RFF03`][RFF03].                   | Componente de persistência do subsistema `GerenciamentoCaronas`.                       |
| `Motorista` (Ator)                | Confirma que o passageiro embarcou.                       | Classe `Motorista`, responsável pela `Carona`, com apoio de `Carona.confirmarEmbarque()`.                 | [`RFU02`][RFU02], [`RFF03`][RFF03], [`RFF06`][RFF06]. | Ator externo representado pelo componente `:Motorista`, usando `:App Motorista`.       |
| **Mensagens / Interações Chave**  |                                                           |                                                                                                           |                                                       |                                                                                        |
| `1: informarChegada()`            | Passageiro informa que chegou ao ponto combinado.         | Atualiza contexto de `Carona` para o passageiro presente.                                                 | [`RFF03`][RFF03].                                     | Comunicação do `Passageiro` com `:App Passageiro`.                                     |
| `2: gerarCodigo()`                | Sistema prepara a confirmação do embarque.                | Método `ValidacaoEmbarque.gerarCodigo()` e atributo `Carona.codigoVerificacao`.                           | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | `:App Passageiro` consome `Ride management interface` de `:Ride API`.                  |
| `3: consultarCarona()`            | Sistema consulta dados da carona e do passageiro.         | Consulta `Carona`, `Motorista`, `Passageiro` e `ValidacaoEmbarque.caronaId`.                              | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | Comunicação de `:Ride API` com `:Banco de dados Carona`.                               |
| `4: dispararNotificacao()`        | Sistema solicita confirmação ao motorista.                | Método `Notificacao.disparar()` com destinatário `Motorista`.                                             | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | `:Notification Service` envia evento para `:Notificação de Carona` e `:App Motorista`. |
| `5: validar()`                    | Motorista confirma o embarque informado.                  | Método `ValidacaoEmbarque.validar(): Boolean`.                                                            | [`RFF03`][RFF03].                                     | Comunicação do `Motorista` via `:App Motorista` com `:Ride API`.                       |
| `6: confirmarEmbarque()`          | Sistema atualiza o estado da carona.                      | Método `Carona.confirmarEmbarque()` e `Carona.status: StatusCarona`.                                      | [`RFF03`][RFF03].                                     | Comunicação de `:Ride API` com `:Banco de dados Carona`.                               |
| `7: registrarLog()`               | Sistema registra o evento no histórico.                   | Método `HistoricoViagem.registrarLog()`.                                                                  | [`RFF03`][RFF03].                                     | Persistência em `:Banco de dados Carona`.                                              |
| `8: exibirConfirmacao()`          | App informa ao passageiro que o embarque foi confirmado.  | Retorno de `Carona.confirmarEmbarque()`.                                                                  | [`RFF03`][RFF03].                                     | Retorno da `Ride management interface` para `:App Passageiro`.                         |

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

> <a id="referencias-bibliograficas-2">2.</a> CARONA AMIGA FCTE. **Protótipo de Alta Fidelidade**. Disponível em: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo. Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> UML Diagrams. **UML Sequence Diagrams Overview**. Disponível em: https://www.uml-diagrams.org/sequence-diagrams.html. Acesso em: 21 set. 2025.

> <a id="referencias-bibliograficas-4">4.</a> CREATELY. **Tutorial do Diagrama de Sequência: Guia completo com exemplos**. Disponível em: https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-sequencia/. Acesso em: 30 abr. 2025.

> <a id="referencias-bibliograficas-5">5.</a> LUCIDCHART. **O que é um diagrama de sequência UML?** Disponível em: https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-sequencia-uml. Acesso em: 30 abr. 2025.

---

## Histórico de versão

| Versão | Data       | Descrição                                                                         | Autor(es)                                                   | Revisor(es)                                                 | Detalhes da Revisão |
| ------ | ---------- | --------------------------------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ------------------- |
| 1.0    | 21/04/2026 | Criação do artefato                                                               | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado   |
| 1.1    | 21/04/2026 | Adição da Introdução, objetivos e metodologia                                     | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado   |
| 1.2    | 22/04/2026 | Adição do modelo do Diagrama de Sequência                                         | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Artefato revisado   |
| 1.3    | 23/04/2026 | Adição do fluxo de confirmação de embarque                                        | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Artefato revisado   |
| 1.4    | 23/04/2026 | Adição dos fluxos de Publicação de carona e Solicitação de participação em carona | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Artefato revisado   |
| 1.5    | 23/04/2026 | Adição dos fluxos E dos Diagramas                                                 | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Artefato revisado   |
