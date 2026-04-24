# Diagrama de Componentes

## Introdução

De acordo com a documentação oficial da UML [[1]](#ref1), o Diagrama de Componentes é um diagrama estrutural que descreve a organização física dos módulos de software, suas **interfaces providas e requeridas** e as **dependências** entre subsistemas. Diferentemente do diagrama de classes, que modela a estrutura lógica, o diagrama de componentes foca nos blocos de construção executáveis ou implantáveis do sistema, como bibliotecas, serviços e módulos, e nos contratos (interfaces) que estabelecem entre si.

A notação bola-e-soquete (*ball-and-socket*) evidencia esses contratos de forma explícita: a **bola** (interface provida) indica o que um componente oferece; o **soquete** (interface requerida) indica o que outro componente consome.

## Tipos Comuns de Diagramas de Componentes

* **Diagrama de visão física:** apresenta como os componentes se organizam em tempo de execução ou implantação.
* **Diagrama de visão lógica:** modela os módulos e subsistemas lógicos e suas dependências conceituais.

No projeto **Carona Amiga**, um web app para conectar motoristas e passageiros, o Diagrama de Componentes é utilizado para evidenciar os subsistemas principais (Backend, autenticação, gerenciamento de caronas, interface, etc.), seus contratos de comunicação e as dependências entre eles, apoiando decisões de arquitetura e facilitando a manutenção do sistema.

## Objetivos

Este artefato tem como finalidade apresentar, de forma clara e estruturada, os módulos do sistema Carona Amiga, seus contratos de interface e relações de dependência. As metas principais são:

- Apresentar o Diagrama de Componentes do web app Carona Amiga, evidenciando subsistemas, interfaces providas/requeridas e dependências;

- Registrar a arquitetura física/lógica do sistema;

- Apoiar o desenvolvimento e a manutenção do sistema ao longo do projeto;

- Servir de referência para checagem/validação dos requisitos arquiteturais elicitados.

---

## Metodologia

1.O **Diagrama de Componentes** foi desenvolvido utilizando a ferramenta [Draw.io](https://app.diagrams.net/), que permite a criação de diagramas UML de forma prática e visual, com suporte à notação bola-e-soquete.

2. Para levantar e justificar os componentes do sistema, foram usadas as informações já consolidadas na [Entrega 01 do projeto](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/), incluindo:

- **Requisitos Funcionais:** para identificar as funcionalidades que cada subsistema deve oferecer;

- **Requisitos Não Funcionais:** para considerar aspectos como segurança, desempenho e escalabilidade, que influenciam a decomposição em componentes;

Informações adicionais, como [5W2H](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/2-Artefato-Generalista/5w2h), [Brainstorming](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/2-Artefato-Generalista/Brainstorm), [Benchmarking](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/2-Artefato-Generalista/Benchmarking) e [Perfil de Usuário](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/5-Iniciativas-Extras/PerfilUsuario), também foram consideradas.

- **Atores do sistema:** [Atores do sistema identificados no Rich Picture](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/2-Artefato-Generalista/1.3.RichPicture);

3. A partir dessas fontes, os componentes foram descritos com suas interfaces e dependências, organizados em subsistemas coerentes com as responsabilidades do sistema.

4. Por fim, o diagrama foi produzido e revisado com base na tabela de verificação, seguindo critérios sintáticos e semânticos da UML.

---

## Composição — Notação UML

<font size="3"><p style="text-align: center">Tabela 1: Legenda do Diagrama de Componentes</p></font>

| Elemento | Símbolo | Descrição |
|---|---|---|
| **Componente** | Retângulo com ícone `<<component>>` | Módulo de software com responsabilidade bem definida. |
| **Interface Provida** | Bola (círculo sólido) | Serviço ou contrato que o componente oferece. |
| **Interface Requerida** | Soquete (semicírculo aberto) | Serviço ou contrato que o componente consome. |
| **Subsistema** | Retângulo com estereótipo `<<subsystem>>` | Agrupamento lógico de componentes relacionados. |
| **Dependência** | `- - - - - - - ►` | Indica que um componente usa outro sem acoplamento permanente. |
| **Realização** | `- - - - - - - ►` com seta aberta | Componente que implementa uma interface. |
| **Conector de montagem** | Bola encaixada no soquete | Liga interface provida de um componente à requerida de outro. |
| **Porta** | Pequeno quadrado na borda | Ponto de interação explícito de um componente com seu exterior. |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Tipos de Relacionamento

Para embasar a escolha dos relacionamentos presentes no diagrama, foi consultado o artigo [What is Component Diagram?](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/). Cada tipo de relacionamento indica um nível diferente de acoplamento entre os componentes do **Carona Amiga**.

<font size="3"><p style="text-align: center">Tabela 2: Tipos de Relacionamentos</p></font>

| Tipo de Relacionamento | O que é | Símbolo | Observação/Extra |
|:-----------------------|:--------|:--------|:-----------------|
| Dependência | Indica que um componente usa outro de forma pontual, sem criar um vínculo permanente. | Linha tracejada com seta. | Representa acoplamento fraco. |
| Realização | Indica que um componente implementa uma interface definida por outro. | Linha tracejada com seta aberta para a interface. | - |
| Conector de montagem | Liga a interface provida de um componente à interface requerida de outro. | Bola encaixada no soquete. | Forma mais comum no diagrama. |
| Delegação | Redireciona uma requisição de uma porta externa a um componente interno. | Seta de delegação. | Usada em componentes compostos. |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

## Conceitos Importantes

### Componente

- **Definição**: Unidade modular e substituível do sistema que encapsula implementação e expõe seu comportamento por meio de interfaces.
- **Exemplo**: O componente `:Auth Service` encapsula toda a lógica de autenticação OAuth2 e expõe a `Authentication interface` para ser consumida pela camada cliente.

### Subsistema

- **Definição**: Agrupamento de componentes com responsabilidades coesas, tratado como uma unidade no diagrama.
- **Exemplo**: O subsistema `GerenciamentoCaronas` agrupa os componentes de pagamento, banco de dados e notificação, todos ligados ao ciclo de vida de uma corrida.

### Interface Provida vs. Requerida

- **Interface Provida**: Contrato que o componente disponibiliza ao exterior (notação: bola).
- **Interface Requerida**: Contrato que o componente precisa que outro forneça (notação: soquete).

---

## Os Relacionamentos no Diagrama de Componentes

<font size="3"><p style="text-align: center">Tabela 3: Multiplicidade e direção das dependências</p></font>

| Relação | Direção | Significado |
|---|---|---|
| Provida → Requerida | Componente A → Componente B | A oferece o que B consome. |
| Delegação interna | Porta → Componente interno | A requisição externa é repassada ao módulo responsável. |
| Dependência estereotipada | `<<criar usuário>>` / `<<validar usuário>>` | Dependência com semântica de negócio explícita. |

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>

---

<div style="text-align: center;">

## Diagrama de Componentes

</div>

<div align="center">
  Figura 1: Diagrama de Componentes.

![Diagrama de componentes](https://i.postimg.cc/2yZ9ThMh/Untitled-Diagram-drawio-(8).png)

<font size="2"><p style="text-align: center">Fonte: [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss) e [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk), 2026.</p></font>
</div>

---

## Descrição dos Subsistemas

O diagrama está organizado em **duas camadas horizontais**:

| Camada | Subsistemas |
|--------|-------------|
| Superior | `Usuários` · `Backend` · `client` |
| Inferior | `GerenciamentoCaronas` · `autentificação` · `interface` |

### `<<subsystem>> Usuários`

Os dois atores principais do sistema.

| Componente | Papel |
|---|---|
| `:Motorista` | Estudante que oferece caronas; consome as interfaces de rastreamento e perfil do Backend. |
| `:Passageiro` | Estudante que solicita caronas; consome as interfaces de perfil e gerenciamento de corridas. |

---

### `<<subsystem>> Backend`

Núcleo do sistema. Expõe **8 interfaces nomeadas** agrupadas por fronteira:

**Interfaces para `Usuários` (esquerda):**

| Interface | Componente provedor |
|---|---|
| `Ride tracking interface` | `:Location Service` |
| `Passenger profile interface` | `:UserService` |

**Interfaces para `client` (direita):**

| Interface | Componente provedor | Protocolo |
|---|---|---|
| `Ride management interface` | `:Ride API` | REST |
| `Admin operations interface` | `:Admin API` | REST |
| `Messaging interface` | `:Chat Service` | WebSocket |
| `Authentication interface` | `:Auth Service` | OAuth2 |

**Interfaces para camada inferior (baixo):**

| Interface | Componente provedor |
|---|---|
| `Ride events interface` | `:Notification Service` |
| `Ride billing interface` | `:Payment Service` |

O `:API Gateway` atua como roteador central, consumindo todas as interfaces internas e delegando às camadas externas.

---

### `<<subsystem>> client`

Camada de apresentação — consome interfaces do Backend.

| Componente | Interfaces consumidas |
|---|---|
| `:Web ADM console` | Admin operations interface |
| `:API Mobile` | Authentication interface · Messaging interface |
| `:App Motorista` | Ride management interface → *Oferece carona* |
| `:App Passageiro` | Ride management interface → *Solicita / Avalia carona* |

---

### `<<subsystem>> GerenciamentoCaronas`

Serviços de suporte operacional às corridas.

| Componente | Responsabilidade |
|---|---|
| `:Payment Service` | Processa pagamentos via `Ride billing interface`. |
| `:Banco de dados Carona` | Persistência lida diretamente pelo API Gateway. |
| `:Notificação de Carona` | Recebe eventos via `Ride events interface`. |

---

### `<<subsystem>> autentificação`

Fluxos de acesso; roteados pelo API Gateway.

| Componente | Responsabilidade |
|---|---|
| `:Login` | Autenticação de usuário existente. |
| `:Cadastro` | Registro de novo usuário (valida e-mail `@fcte.unb.br`). |
| `:Recuperação de senha` | Redefinição via link enviado por e-mail. |

> O `:Auth Service` (Backend) comunica-se diretamente com `:Motorista` e `:Passageiro` via dependências estereotipadas `<<criar usuário>>` e `<<validar usuário>>`.

---

### `<<subsystem>> interface`

Camada de interação com avaliações e perfil do usuário.

| Componente | Interface consumida | Ação |
|---|---|---|
| `:Avaliação` | Ride events interface | Submete avaliação pós-corrida. |
| `:Carona` | Ride management interface | Consulta/exibe detalhes da corrida. |
| `:Perfil` | Passenger profile interface | Exibe e edita perfil público. |

---


## Reunião de Alinhamento sobre o diagrama de componentes

<iframe width="1321" height="743" src="https://youtu.be/gsj8lC_sC0s" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/gsj8lC_sC0s" target="_blank">Clique aqui para assistir no YouTube</a></p>


---

## Conclusão

A elaboração do Diagrama de Componentes do projeto **Carona Amiga** permitiu representar, de forma estruturada, os principais módulos do sistema, seus contratos de interface e as dependências entre subsistemas. O artefato contribui para o alinhamento arquitetural da equipe e para a rastreabilidade entre requisitos e implementação. Dessa forma, o diagrama também se torna uma referência para evolução, manutenção e tomada de decisões técnicas ao longo do projeto.

---

## Referências Bibliográficas

> <a id="ref1"></a>1. UML Diagrams. *Component Diagrams Overview*. Disponível em: https://www.uml-diagrams.org/component-diagrams.html. Acesso em: 20 abr. 2026.
>
> <a id="ref2"></a>2. Visual Paradigm. *What is Component Diagram?*. Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/what-is-component-diagram/. Acesso em: 20 abr. 2026.
>
> <a id="ref3"></a>3. Aula Modelagem UML Estática. Material de aula. 2026.

---

## Histórico de Versões

| Versão | Data | Descrição | Autor | Revisor |
| :----: | :--: | --------- | ------ | ------ |
| 1.0 | 16/04/2026 | Criação do Diagrama de Componentes | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa)
| 1.1 | 16/04/2026 | Refatoração para notação UML ball-and-socket com subsistemas | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharesss)
| 1.2 | 20/04/2026 | Reestruturação do documento com introdução, metodologia, legenda e descrição dos subsistemas | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk)
