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

A elaboração dos diagramas de sequência do **Carona Amiga FCTE** seguirá uma abordagem iterativa, com base nos artefatos previamente construídos pela equipe, especialmente no diagrama de classes <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-6">[6]</a>, no diagrama de comunicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-7">[7]</a> e nos fluxos definidos no protótipo de alta fidelidade da aplicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>. Essa rastreabilidade permite relacionar a estrutura estática do sistema, a colaboração entre os participantes e a navegação prevista para o usuário. A partir desses artefatos, o comportamento do sistema será observado sob a perspectiva temporal das interações, permitindo identificar a ordem das mensagens trocadas entre os atores, a interface, os serviços internos e a persistência dos dados.

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
6. Revisão dos diagramas com base nos demais artefatos do projeto, especialmente no diagrama de classes <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-6">[6]</a>, no diagrama de comunicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-7">[7]</a> e no protótipo de alta fidelidade <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>, para manter coerência entre a modelagem estática, a modelagem dinâmica e os fluxos de navegação previstos;
7. Verificação final por meio de checklist, considerando critérios de consistência, completude, clareza e conformidade com a UML.

Dessa forma, a metodologia adotada permite que os diagramas de sequência sejam derivados de fluxos reais de uso da aplicação, mantendo rastreabilidade com o protótipo de alta fidelidade <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-2">[2]</a>, com o diagrama de classes <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-6">[6]</a> e com o diagrama de comunicação <a href="#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_sequencia?id=referencias-bibliograficas-7">[7]</a>, apoiando a validação do comportamento esperado do sistema **Carona Amiga FCTE**.

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

### Apresentação dos Diagramas de Sequência

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

| Elemento do Diagrama de Sequência           | Descrição na Sequência                                                   | Relação com Diagrama de Classes                                                                        | Relação com Requisitos (RFs)                          | Relação com Diagrama de Componentes                                           |
| :------------------------------------------ | :----------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------- | :---------------------------------------------------- | :---------------------------------------------------------------------------- |
| **Lifelines / Participantes**               |                                                                          |                                                                                                        |                                                       |                                                                               |
| `Usuário` (Ator)                            | Acessa a tela, preenche o cadastro e recebe o retorno do processo.       | Instância de `Usuario`; pode se especializar em `Motorista` ou `Passageiro`.                           | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS02`][RFS02]. | Ator externo representado pelos apps cliente do sistema.                      |
| `:App Passageiro / App Driver`              | Exibe o formulário de cadastro, coleta os dados e mostra feedback.       | Interface de entrada para atributos de `Usuario`, `PreferenciaPareamento` e, quando houver, `Veiculo`. | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS01`][RFS01]. | Componente do subsistema `Client`.                                            |
| `:API Mobile`                               | Recebe os dados do aplicativo e encaminha a solicitação ao backend.      | Transporta dados de criação de `Usuario`.                                                              | [`RFS02`][RFS02].                                     | Componente do cliente conectado à `Authentication interface`.                 |
| `:Authentication Interface`                 | Expõe a operação de cadastro para autenticação do usuário.               | Encaminha a criação de `Usuario` ao serviço de autenticação.                                           | [`RFS02`][RFS02].                                     | Interface de autenticação entre cliente e backend.                            |
| `:Auth Service`                             | Orquestra a criação da conta e aciona a validação do cadastro.           | Relaciona-se à operação de criação de `Usuario` e ao controle de vínculo institucional.                | [`RFS02`][RFS02].                                     | Componente do backend que provê `Authentication interface`.                   |
| `:Cadastro`                                 | Valida os dados informados e decide entre erro ou continuidade do fluxo. | Centraliza validações de `Usuario`, incluindo `emailInstitucional`.                                    | [`RFS01`][RFS01], [`RFS02`][RFS02].                   | Componente do subsistema `Authentication`.                                    |
| `:UserService`                              | Cria o perfil do usuário e salva dados complementares e conta final.     | Manipula `Usuario`, `PreferenciaPareamento` e `Veiculo`.                                               | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS01`][RFS01]. | Componente do backend responsável por perfil de usuário.                      |
| `:Banco de Dados`                           | Verifica e-mail institucional e persiste os registros do cadastro.       | Persiste `Usuario`, `PreferenciaPareamento` e `Veiculo`.                                               | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFS02`][RFS02]. | Camada de persistência do sistema.                                            |
| **Mensagens / Interações Chave**            |                                                                          |                                                                                                        |                                                       |                                                                               |
| `1: acessaTelaCadastro()/exibeFormulario()` | O app apresenta a tela de cadastro para início do fluxo.                 | Interface inicial de criação de `Usuario`.                                                             | [`RFS01`][RFS01], [`RFS02`][RFS02].                   | Comunicação entre `Usuário` e `:App Passageiro / App Driver`.                 |
| `2: enviarDadosCadastro()`                  | Os dados preenchidos seguem do app até a `Authentication Interface`.     | Encaminha os atributos de `Usuario` para cadastro.                                                     | [`RFS02`][RFS02].                                     | Fluxo `Client -> API Mobile -> Authentication Interface`.                     |
| `3: createUser()/validarDados()`            | O backend inicia a criação da conta e valida os dados informados.        | Relaciona-se a `Usuario.cadastrar()` e à validação de `emailInstitucional`.                            | [`RFS02`][RFS02].                                     | Comunicação entre `:Authentication Interface`, `:Auth Service` e `:Cadastro`. |
| `4: verificarEmailInstitucional()`          | O sistema verifica se o e-mail é válido e se não há conflito cadastral.  | Usa `Usuario.emailInstitucional`.                                                                      | [`RFS02`][RFS02].                                     | `:Cadastro` consulta `:Banco de Dados`.                                       |
| `5: erroCadastro()/cadastroNegado()`        | Em caso de erro, o motivo retorna até a interface do usuário.            | Retorno negativo da criação de `Usuario`.                                                              | [`RFS02`][RFS02].                                     | Retorno encadeado do backend até `:App Passageiro / App Driver`.              |
| `6: criarPerfil()`                          | Com dados válidos, o sistema cria o perfil básico do usuário.            | Manipula `Usuario` e inicializa dados de perfil.                                                       | [`RFS01`][RFS01], [`RFS02`][RFS02].                   | `:Cadastro` aciona `:UserService`.                                            |
| `7: salvarDadosComplementares()`            | Quando houver veículo, CNH ou preferências, os dados extras são salvos.  | Persiste `Veiculo` e `PreferenciaPareamento`.                                                          | [`RFU01`][RFU01], [`RFU02`][RFU02].                   | `:UserService` consulta/persiste em `:Banco de Dados`.                        |
| `8: salvarUsuario()/cadastroRealizado()`    | O usuário é salvo e o sucesso retorna até a interface.                   | Persistência final de `Usuario`.                                                                       | [`RFS02`][RFS02].                                     | Retorno encadeado de `:UserService` até o app cliente.                        |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 1, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 1: Diagrama de Sequência - Cadastro de usuário
    <br>
    <img src="assets/diagramas/diagrama_sequencia_cadastro.png">
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

| Elemento do Diagrama de Sequência               | Descrição na Sequência                                               | Relação com Diagrama de Classes                                          | Relação com Requisitos (RFs) | Relação com Diagrama de Componentes                                        |
| :---------------------------------------------- | :------------------------------------------------------------------- | :----------------------------------------------------------------------- | :--------------------------- | :------------------------------------------------------------------------- |
| **Lifelines / Participantes**                   |                                                                      |                                                                          |                              |                                                                            |
| `Usuário Cadastrado` (Ator)                     | Acessa a tela de login, informa credenciais e recebe a resposta.     | Instância já registrada de `Usuario`, `Motorista` ou `Passageiro`.       | [`RFS02`][RFS02].            | Ator externo representado pelos apps cliente.                              |
| `:App Passageiro / App Driver`                  | Exibe o formulário de login, envia credenciais e mostra o resultado. | Interface usada para autenticação de `Usuario`.                          | [`RFS02`][RFS02].            | Componente do subsistema `Client`.                                         |
| `:API Mobile`                                   | Encaminha as credenciais para a camada de autenticação.              | Transporta os dados de `Usuario.login()`.                                | [`RFS02`][RFS02].            | Componente cliente integrado à autenticação.                               |
| `:Authentication Interface`                     | Expõe a operação de login para o backend.                            | Encaminha o acesso de `Usuario` ao serviço de autenticação.              | [`RFS02`][RFS02].            | Interface entre cliente e backend.                                         |
| `:Auth Service`                                 | Valida o usuário e coordena o retorno de erro ou sucesso.            | Verifica dados de `Usuario`.                                             | [`RFS02`][RFS02].            | Componente do backend que provê `Authentication interface`.                |
| `:Login`                                        | Executa a autenticação e consulta o usuário pelo e-mail.             | Aciona `Usuario.login()` com `emailInstitucional` e `senhaHash`.         | [`RFS02`][RFS02].            | Componente do subsistema `Authentication`.                                 |
| `:UserService`                                  | Carrega o perfil completo após autenticação válida.                  | Consulta `Usuario`, `Motorista`, `Passageiro` e `PreferenciaPareamento`. | [`RFS02`][RFS02].            | Serviço responsável por dados de perfil.                                   |
| `:Banco de Dados`                               | Retorna os dados do usuário e do perfil consultado.                  | Persiste e consulta `Usuario` e dados associados.                        | [`RFS02`][RFS02].            | Camada de persistência do sistema.                                         |
| **Mensagens / Interações Chave**                |                                                                      |                                                                          |                              |                                                                            |
| `1: acessaTelaLogin()/exibeFormulario()`        | O aplicativo apresenta a tela de login ao usuário.                   | Interface inicial para `Usuario.login()`.                                | [`RFS02`][RFS02].            | Comunicação entre `Usuário Cadastrado` e `:App Passageiro / App Driver`.   |
| `2: enviarCredenciais()`                        | O app envia e-mail e senha até a `Authentication Interface`.         | Usa `Usuario.emailInstitucional` e `Usuario.senhaHash`.                  | [`RFS02`][RFS02].            | Fluxo `Client -> API Mobile -> Authentication Interface`.                  |
| `3: validateUser()/autenticar()`                | O backend valida as credenciais informadas.                          | Execução de `Usuario.login(): Boolean`.                                  | [`RFS02`][RFS02].            | Comunicação entre `:Authentication Interface`, `:Auth Service` e `:Login`. |
| `4: buscarUsuarioPorEmail()`                    | O componente de login consulta os dados básicos do usuário.          | Consulta `Usuario` persistido.                                           | [`RFS02`][RFS02].            | `:Login` consulta `:Banco de Dados`.                                       |
| `5: erroAutenticacao()/loginNegado()`           | Quando as credenciais são inválidas, o erro retorna até o app.       | Retorno negativo de `Usuario.login()`.                                   | [`RFS02`][RFS02].            | Retorno encadeado do backend até a interface do usuário.                   |
| `6: carregarPerfil()/consultarPerfil()`         | Com login válido, o sistema busca o perfil completo do usuário.      | Usa dados de `Usuario`, `Motorista` ou `Passageiro`.                     | [`RFS02`][RFS02].            | Comunicação entre `:Login`, `:UserService` e `:Banco de Dados`.            |
| `7: usuarioAutenticado()/sessaoAtiva()`         | O token e o tipo de usuário retornam para abertura da sessão.        | Sucesso da autenticação de `Usuario`.                                    | [`RFS02`][RFS02].            | Retorno de `:Login` até `:API Mobile`.                                     |
| `8: retornaAcesso()/liberaAcessoAoAplicativo()` | O app libera a entrada do usuário autenticado.                       | Retorno positivo de `Usuario.login()`.                                   | [`RFS02`][RFS02].            | Resultado final apresentado ao ator no cliente.                            |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 2, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 2: Diagrama de Sequência - Login
    <br>
    <img src="assets/diagramas/diagrama_sequencia_login.png">
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

| Elemento do Diagrama de Sequência                | Descrição na Sequência                                                  | Relação com Diagrama de Classes                                          | Relação com Requisitos (RFs)                                            | Relação com Diagrama de Componentes                          |
| :----------------------------------------------- | :---------------------------------------------------------------------- | :----------------------------------------------------------------------- | :---------------------------------------------------------------------- | :----------------------------------------------------------- |
| **Lifelines / Participantes**                    |                                                                         |                                                                          |                                                                         |                                                              |
| `Passageiro` (Ator)                              | Acessa a busca, informa filtros e visualiza os resultados.              | Especialização de `Usuario` com preferências de pareamento.              | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Ator externo representado pelo componente `:Passageiro`.     |
| `:App Passageiro`                                | Exibe os filtros de busca e apresenta a ausência ou a lista de caronas. | Interface que mostra dados de `Carona`, `Rota` e informações associadas. | [`RFM02`][RFM02], [`RFS01`][RFS01], [`RFS03`][RFS03].                   | Componente do subsistema `Client`.                           |
| `:API Mobile`                                    | Encaminha os filtros de busca para a interface de viagens.              | Transporta a consulta de caronas no fluxo móvel.                         | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | Componente intermediário entre app e backend.                |
| `:Ride Interface`                                | Expõe a operação de consulta de caronas para o backend.                 | Encaminha a busca de `Carona` com base nos filtros recebidos.            | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | Interface de gerenciamento de caronas.                       |
| `:Ride API`                                      | Coordena validação de localização, rota e disponibilidade de caronas.   | Coordena consulta de `Carona`, `Rota` e regras de disponibilidade.       | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Componente do backend que provê `Ride management interface`. |
| `:LocationService`                               | Valida origem/destino informados pelo passageiro.                       | Usa `Localização` e seus dados geográficos.                              | [`RFM01`][RFM01].                                                       | Serviço de localização do backend.                           |
| `:Rota`                                          | Calcula a rota a partir da origem e do destino informados.              | Relaciona-se à classe `Rota` e seus cálculos de percurso.                | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Elemento de domínio usado pelo backend na busca.             |
| `:Carona`                                        | Filtra as caronas pela disponibilidade de vagas e status.               | Usa atributos `status` e `vagasDisponiveis` de `Carona`.                 | [`RFM01`][RFM01], [`RFM02`][RFM02], [`RFF02`][RFF02].                   | Elemento de domínio usado na seleção das opções disponíveis. |
| `:Banco de Dados`                                | Retorna a lista de caronas consultadas com base em filtros e rota.      | Persiste `Carona`, `Motorista`, `Avaliacao`, `Rota` e `Localização`.     | [`RFS03`][RFS03], [`RFF07`][RFF07].                                     | Camada de persistência do sistema.                           |
| **Mensagens / Interações Chave**                 |                                                                         |                                                                          |                                                                         |                                                              |
| `1: acessaBusca()/exibeFiltros()`                | O passageiro abre a busca e o app apresenta os campos de filtragem.     | Interface de entrada de critérios para consulta de `Carona`.             | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | Comunicação entre `Passageiro` e `:App Passageiro`.          |
| `2: informarFiltros()/buscarCaronas()`           | Os filtros seguem do app até a `Ride Interface`.                        | Encaminha critérios de busca relacionados a `Carona` e `Rota`.           | [`RFU02`][RFU02], [`RFM01`][RFM01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | Fluxo `:App Passageiro -> :API Mobile -> :Ride Interface`.   |
| `3: buscarCaronasDisponiveis()`                  | A `Ride API` recebe a solicitação principal de busca.                   | Inicia a consulta de objetos `Carona`.                                   | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | `:Ride Interface` aciona `:Ride API`.                        |
| `4: validarLocalizacao()`                        | O sistema valida origem e destino antes de calcular a rota.             | Usa dados de `Localização`.                                              | [`RFM01`][RFM01].                                                       | Comunicação entre `:Ride API` e `:LocationService`.          |
| `5: calcularRota()`                              | A rota é calculada para apoiar a consulta de caronas.                   | Usa `Rota.calcularRota()` e informações de percurso.                     | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Comunicação entre `:Ride API` e `:Rota`.                     |
| `6: consultarCaronas()/listaCaronas()`           | O backend consulta o banco de dados com filtros e rota.                 | Consulta `Carona` persistida com base em status e contexto.              | [`RFM01`][RFM01], [`RFF07`][RFF07].                                     | `:Ride API` consulta `:Banco de Dados`.                      |
| `7: verificarStatusEVagas()`                     | As caronas retornadas são filtradas pela disponibilidade real.          | Usa `Carona.status` e `Carona.vagasDisponiveis`.                         | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Comunicação entre `:Ride API` e `:Carona`.                   |
| `8: listaVazia()/semResultados()`                | Quando não há caronas compatíveis, o sistema devolve lista vazia.       | Retorno sem instâncias válidas de `Carona`.                              | [`RFF07`][RFF07].                                                       | Retorno encadeado até `:App Passageiro`.                     |
| `9: listaCaronasDisponiveis()/resultadosBusca()` | Quando há opções, os resultados voltam até a interface.                 | Retorno das `Carona` disponíveis para exibição.                          | [`RFM02`][RFM02], [`RFS03`][RFS03].                                     | Retorno final de `:Ride API` até o `Passageiro`.             |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/navicg">Ana Victória Guedes da Costa</a>, 2026.
</div>

Com base na tabela 3, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 3: Diagrama de Sequência - Busca de caronas
    <br>
    <img src="assets/diagramas/diagrama_sequencia_busca.png">
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

| Elemento do Diagrama de Sequência      | Descrição na Sequência                                                        | Relação com Diagrama de Classes                                                                                                  | Relação com Requisitos (RFs)                                            | Relação com Diagrama de Componentes                                     |
| :------------------------------------- | :---------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------- |
| **Lifelines / Participantes**          |                                                                               |                                                                                                                                  |                                                                         |                                                                         |
| `Passageiro` (Ator)                    | Seleciona a carona, solicita participação e recebe a confirmação do envio.    | Classe `Passageiro`, especialização de `Usuario`, associada à operação `solicitarCarona()`.                                      | [`RFU02`][RFU02], [`RFM02`][RFM02], [`RFF01`][RFF01].                   | Ator externo representado pelo componente `:Passageiro`.                |
| `:App Passageiro`                      | Exibe os detalhes da carona e encaminha a solicitação ao backend.             | Interface que apresenta dados de `Carona`, `Motorista` e preferências do passageiro.                                             | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Componente cliente que consome a interface de gerenciamento de caronas. |
| `:API Gateway`                         | Encaminha a solicitação de participação para a API de caronas.                | Transporta a chamada de `Passageiro.solicitarCarona()`.                                                                          | [`RFF01`][RFF01], [`RFF07`][RFF07].                                     | Camada intermediária entre o app e a `Ride API`.                        |
| `:Ride API`                            | Processa a solicitação, consulta a carona, aplica regras e registra o pedido. | Coordena `Passageiro.solicitarCarona()`, `PreferenciaPareamento.aplicarFiltro(Carona[*])` e atualização de `Carona.passageiros`. | [`RFU02`][RFU02], [`RFF01`][RFF01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | Componente do backend que provê `Ride management interface`.            |
| `:Banco de dados Carona`               | Retorna a carona consultada e persiste a solicitação registrada.              | Persiste `Carona`, `Passageiro` associado e atualização de `vagasDisponiveis`.                                                   | [`RFU02`][RFU02], [`RFF01`][RFF01].                                     | Camada de persistência do gerenciamento de caronas.                     |
| `:Notification Service`                | Dispara a notificação de nova solicitação para o motorista.                   | Relaciona-se ao envio de `Notificacao` para análise do pedido.                                                                   | [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Serviço de notificação do backend.                                      |
| `:App Motorista`                       | Recebe a notificação e exibe o pedido ao motorista.                           | Interface usada pelo `Motorista` para visualizar solicitações recebidas.                                                         | [`RFF06`][RFF06].                                                       | Componente cliente do motorista.                                        |
| `Motorista` (Ator)                     | Recebe a notificação da nova solicitação enviada pelo passageiro.             | Classe `Motorista`, responsável pela `Carona`.                                                                                   | [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Ator externo representado pelo componente `:Motorista`.                 |
| **Mensagens / Interações Chave**       |                                                                               |                                                                                                                                  |                                                                         |                                                                         |
| `1: selecionarCarona()`                | O passageiro escolhe a carona desejada no aplicativo.                         | Consulta uma instância de `Carona` associada ao `Motorista`.                                                                     | [`RFM02`][RFM02], [`RFF02`][RFF02].                                     | Comunicação entre `Passageiro` e `:App Passageiro`.                     |
| `2: solicitarCarona(idCarona)`         | O app envia a solicitação de participação ao `API Gateway`.                   | Aciona `Passageiro.solicitarCarona()`.                                                                                           | [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Fluxo `:App Passageiro -> :API Gateway -> :Ride API`.                   |
| `3: consultarCarona()/aplicarFiltro()` | A `Ride API` consulta a carona e verifica preferências e disponibilidade.     | Usa `PreferenciaPareamento.aplicarFiltro(Carona[*])` e consulta `Carona.vagasDisponiveis`.                                       | [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Processamento interno da `:Ride API` com consulta ao banco.             |
| `4: registrarPassageiro()`             | O sistema persiste a solicitação registrada na carona.                        | Atualiza `Carona.passageiros` e o vínculo do passageiro com a viagem.                                                            | [`RFF01`][RFF01].                                                       | Comunicação entre `:Ride API` e `:Banco de dados Carona`.               |
| `5: dispararNotificacao()`             | O backend notifica o motorista sobre a nova solicitação.                      | Relaciona-se ao envio de `Notificacao` para o `Motorista`.                                                                       | [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Fluxo `:Ride API -> :Notification Service -> :App Motorista`.           |
| `6: exibirSolicitacaoEnviada()`        | O retorno de sucesso volta ao app e é exibido ao passageiro.                  | Retorno da execução bem-sucedida de `Passageiro.solicitarCarona()`.                                                              | [`RFF01`][RFF01].                                                       | Resultado final apresentado por `:App Passageiro` ao ator.              |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>
Com base na tabela 4, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 4: Diagrama de Sequência - Solicitação de participação em carona
    <br>
    <img src="assets/diagramas/diagrama_sequencia-solicitacao-carona.png">
    <br>
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>.
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

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                   | Relação com Diagrama de Classes                                                                                                                     | Relação com Requisitos (RFs)                                                              | Relação com Diagrama de Componentes                          |
| :-------------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :----------------------------------------------------------- |
| **Lifelines / Participantes**     |                                                                          |                                                                                                                                                     |                                                                                           |                                                              |
| `Motorista` (Ator)                | Abre a publicação, informa os dados da viagem e recebe a confirmação.    | Classe `Motorista`, especialização de `Usuario`, associada a `Veiculo` e `Carona`.                                                                  | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF06`][RFF06].                                     | Ator externo representado pelo componente `:Motorista`.      |
| `:App Motorista`                  | Exibe o formulário de publicação e envia os dados preenchidos.           | Interface que aciona `Motorista.publicarCarona()` e apresenta dados de `Carona`, `Veiculo` e `Rota`.                                                | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Componente cliente do motorista.                             |
| `:API Gateway`                    | Encaminha a publicação da carona ao backend.                             | Transporta a chamada `publicarCarona(dadosCarona)`.                                                                                                 | [`RFF01`][RFF01].                                                                         | Camada intermediária entre app e `Ride API`.                 |
| `:Ride API`                       | Valida o motorista, o veículo, a rota e publica a nova carona.           | Coordena `Motorista.validarCarona()`, `Veiculo.validarDocumentacao(placa)`, `PreferenciaPareamento.aplicarFiltro(Carona[*])` e `Carona.publicar()`. | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF01`][RFF01], [`RFF06`][RFF06], [`RFF07`][RFF07]. | Componente do backend que provê `Ride management interface`. |
| `:Location Service`               | Calcula rota e tempo estimado para a carona publicada.                   | Usa `Rota.calcularRota(Array Localizacao[])` e `Rota.calcularTempoEstimadoMin(Array pontos)`.                                                       | [`RFM01`][RFM01], [`RFM02`][RFM02].                                                       | Serviço de localização do backend.                           |
| `:Banco de dados Carona`          | Persiste a nova carona publicada e confirma o registro.                  | Persiste `Carona`, `Motorista`, `Veiculo`, `Rota`, `Localização` e `StatusCarona`.                                                                  | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Camada de persistência do gerenciamento de caronas.          |
| **Mensagens / Interações Chave**  |                                                                          |                                                                                                                                                     |                                                                                           |                                                              |
| `1: abrirPublicacao()`            | O motorista acessa a funcionalidade de publicar carona.                  | Operação iniciada por `Motorista`.                                                                                                                  | [`RFU01`][RFU01].                                                                         | Comunicação entre `Motorista` e `:App Motorista`.            |
| `2: preencherDadosCarona()`       | O motorista informa origem, destino, horário, vagas e custo.             | Preenche atributos de `Carona`, como `origem`, `destino`, `horarioPartida`, `vagasDisponiveis` e `precoBase`.                                       | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Interação direta do ator com `:App Motorista`.               |
| `3: publicarCarona(dadosCarona)`  | O app encaminha os dados para `API Gateway` e `Ride API`.                | Aciona `Motorista.publicarCarona()` e prepara a criação de `Carona`.                                                                                | [`RFF01`][RFF01], [`RFF02`][RFF02].                                                       | Fluxo `:App Motorista -> :API Gateway -> :Ride API`.         |
| `4: validarCarona()`              | A `Ride API` valida motorista, documentação, rota, tempo e preferências. | Usa `Motorista.validarCarona()`, `Veiculo.validarDocumentacao(placa)`, `Rota.calcularRota()` e `PreferenciaPareamento.aplicarFiltro(Carona[*])`.    | [`RFU01`][RFU01], [`RFU02`][RFU02], [`RFF06`][RFF06], [`RFF07`][RFF07].                   | Processamento interno com apoio do `:Location Service`.      |
| `5: salvarCarona()`               | Após validação, a nova carona é persistida no banco de dados.            | Persiste `Carona.status`, `motorista` e dados de rota/localização.                                                                                  | [`RFM01`][RFM01], [`RFF01`][RFF01], [`RFF02`][RFF02].                                     | Comunicação entre `:Ride API` e `:Banco de dados Carona`.    |
| `6: confirmarPublicacao()`        | O retorno de sucesso volta ao aplicativo e é exibido ao motorista.       | Retorno da execução de `Carona.publicar()`.                                                                                                         | [`RFF01`][RFF01].                                                                         | Resultado final apresentado por `:App Motorista` ao ator.    |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>

Com base na tabela 5, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 5: Diagrama de Sequência - Publicação de carona
    <br>
    <img src="assets/diagramas/diagrama_sequencia_publicacao-carona.png">
    <br>
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>.
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

| Elemento do Diagrama de Sequência | Descrição na Sequência                                                 | Relação com Diagrama de Classes                                                                           | Relação com Requisitos (RFs)                          | Relação com Diagrama de Componentes                                             |
| :-------------------------------- | :--------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------ |
| **Lifelines / Participantes**     |                                                                        |                                                                                                           |                                                       |                                                                                 |
| `Passageiro` (Ator)               | Informa chegada ao ponto de embarque e recebe a confirmação final.     | Classe `Passageiro`, especialização de `Usuario`, vinculada à `Carona.passageiros`.                       | [`RFU02`][RFU02], [`RFF03`][RFF03].                   | Ator externo representado pelo componente `:Passageiro`.                        |
| `:App Passageiro`                 | Encaminha a chegada e exibe o resultado da confirmação.                | Interface que apresenta dados de `Carona`, `ValidacaoEmbarque` e `StatusCarona`.                          | [`RFF03`][RFF03].                                     | Componente cliente do passageiro.                                               |
| `:API Gateway`                    | Encaminha operações de geração e validação do embarque.                | Transporta as chamadas `gerarCodigo()` e `validar()`.                                                     | [`RFU02`][RFU02], [`RFF03`][RFF03].                   | Camada intermediária entre app e `Ride API`.                                    |
| `:Ride API`                       | Consulta dados, gera código, valida confirmação e atualiza o embarque. | Coordena `ValidacaoEmbarque.gerarCodigo()`, `ValidacaoEmbarque.validar()` e `Carona.confirmarEmbarque()`. | [`RFU02`][RFU02], [`RFF03`][RFF03], [`RFF06`][RFF06]. | Componente do backend que provê `Ride management interface`.                    |
| `:Banco de dados Carona`          | Retorna dados da carona e persiste atualização e log do embarque.      | Persiste `Carona`, `ValidacaoEmbarque`, `StatusCarona` e `HistoricoViagem`.                               | [`RFU02`][RFU02], [`RFF03`][RFF03].                   | Camada de persistência do gerenciamento de caronas.                             |
| `:Notification Service`           | Solicita a confirmação do embarque ao motorista.                       | Relaciona-se ao envio de `Notificacao` de confirmação.                                                    | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | Serviço de notificação do backend.                                              |
| `:App Motorista`                  | Exibe a solicitação de confirmação e envia a validação.                | Interface usada pelo `Motorista` para confirmar o embarque.                                               | [`RFF03`][RFF03].                                     | Componente cliente do motorista.                                                |
| `Motorista` (Ator)                | Confirma que o passageiro embarcou.                                    | Classe `Motorista`, responsável pela `Carona`, com apoio de `Carona.confirmarEmbarque()`.                 | [`RFU02`][RFU02], [`RFF03`][RFF03], [`RFF06`][RFF06]. | Ator externo representado pelo componente `:Motorista`.                         |
| **Mensagens / Interações Chave**  |                                                                        |                                                                                                           |                                                       |                                                                                 |
| `1: informarChegada()`            | O passageiro informa que chegou ao ponto de embarque.                  | Atualiza o contexto de `Carona` para o passageiro presente.                                               | [`RFF03`][RFF03].                                     | Comunicação entre `Passageiro` e `:App Passageiro`.                             |
| `2: gerarCodigo()`                | O app solicita ao backend a geração do código de embarque.             | Usa `ValidacaoEmbarque.gerarCodigo()` e `Carona.codigoVerificacao`.                                       | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | Fluxo `:App Passageiro -> :API Gateway -> :Ride API`.                           |
| `3: consultarCarona()`            | A `Ride API` consulta os dados da carona e do passageiro.              | Consulta `Carona`, `Motorista`, `Passageiro` e dados de validação.                                        | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | Comunicação entre `:Ride API` e `:Banco de dados Carona`.                       |
| `4: dispararNotificacao()`        | O sistema envia ao motorista a solicitação de confirmação.             | Usa `Notificacao` para avisar o `Motorista` via app.                                                      | [`RFU02`][RFU02], [`RFF06`][RFF06].                   | Fluxo `:Ride API -> :Notification Service -> :App Motorista`.                   |
| `5: validar()`                    | O motorista confirma a solicitação no aplicativo.                      | Executa `ValidacaoEmbarque.validar()`.                                                                    | [`RFF03`][RFF03].                                     | Fluxo `Motorista -> :App Motorista -> :API Gateway -> :Ride API`.               |
| `6: confirmarEmbarque()`          | O backend atualiza o estado do embarque na carona.                     | Usa `Carona.confirmarEmbarque()` e atualiza `Carona.status`.                                              | [`RFF03`][RFF03].                                     | Comunicação entre `:Ride API` e `:Banco de dados Carona`.                       |
| `7: registrarLog()`               | O evento de confirmação é registrado no histórico.                     | Usa `HistoricoViagem.registrarLog()`.                                                                     | [`RFF03`][RFF03].                                     | Persistência adicional em `:Banco de dados Carona`.                             |
| `8: exibirConfirmacao()`          | O resultado da confirmação volta ao passageiro e ao motorista.         | Retorno positivo da validação de embarque.                                                                | [`RFF03`][RFF03].                                     | Resultado final exibido por `:App Passageiro` e registrado em `:App Motorista`. |

<div align="center">
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>, 2026.
</div>

Com base na tabela 6, abaixo está apresentado o diagrama de sequência correspondente.

<div align="center">
    Figura 6: Diagrama de Sequência - Confirmação de embarque
    <br>
    <img src="assets/diagramas/diagrama_sequencia-confirm-embarque.png">
    <br>
    <b>Autora:</b> <a href="https://github.com/KarolineLuz">Karoline Luz da Conceição</a>.
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

> <a id="referencias-bibliograficas-6">6.</a> CARONA AMIGA FCTE. **Diagrama de Classes**. Disponível em: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_02/#/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-7">7.</a> CARONA AMIGA FCTE. **Diagrama de Comunicação**. Disponível em: https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_02/#/Modelagem/2.2.ModelagemDinamica/Diagrama_de_comunicacao. Acesso em: 23 abr. 2026.

---

## Histórico de versão

| Versão | Data       | Descrição                                                                          | Autor(es)                                                   | Revisor(es)                                                 | Detalhes da Revisão |
| ------ | ---------- | ---------------------------------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ------------------- |
| 1.0    | 21/04/2026 | Criação do artefato                                                                | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Revisão inicial da estrutura, do escopo e da organização do documento. |
| 1.1    | 21/04/2026 | Adição da Introdução, objetivos e metodologia                                      | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Verificação da clareza textual, da coerência metodológica e do alinhamento com a proposta do artefato. |
| 1.2    | 22/04/2026 | Adição do modelo do Diagrama de Sequência                                          | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Revisão da representação dos participantes, da ordem das mensagens e da aderência à notação UML. |
| 1.3    | 23/04/2026 | Adição do fluxo de confirmação de embarque                                         | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Análise da consistência do fluxo, com foco nas validações, retornos e atualização de estados da carona. |
| 1.4    | 23/04/2026 | Adição dos fluxos de publicação de carona e solicitação de participação em carona  | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Revisão da completude dos cenários, das interações entre ator e sistema e da compatibilidade com os requisitos funcionais. |
| 1.5    | 23/04/2026 | Consolidação dos fluxos e inclusão dos respectivos diagramas                       | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Conferência da correspondência entre descrição textual, tabelas explicativas e diagramas apresentados. |
| 1.6    | 23/04/2026 | Adição dos diagramas de sequência relacionados a cadastro, login e busca de carona | [Ana Victória Guedes da Costa](https://github.com/navicg)   | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Revisão da legibilidade dos fluxos principais e da coerência entre entradas, processamentos e respostas exibidas ao usuário. |
| 1.7    | 23/04/2026 | Adição correta da rastreabilidade                                                  | [Karoline Luz da Conceição](https://github.com/KarolineLuz) | [Ana Victória Guedes da Costa](https://github.com/navicg)   | Validação final das referências cruzadas com requisitos, diagrama de classes, diagrama de comunicação e protótipo. |
