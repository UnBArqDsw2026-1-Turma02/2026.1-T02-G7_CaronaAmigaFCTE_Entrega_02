## Introdução

O Diagrama de Casos de Uso integra o conjunto de diagramas comportamentais da UML (Unified Modeling Language) e tem como finalidade representar, de maneira clara, as funcionalidades de um sistema sob a ótica dos usuários. De acordo com a literatura especializada, como apresentado pela [Lucidchart](https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml), esse tipo de diagrama permite identificar os atores envolvidos — sejam eles usuários ou sistemas externos — e explicitar as interações realizadas com o sistema, facilitando a compreensão do seu funcionamento.

Além disso, conforme destacado pelo site da [DevMedia](https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408)[[1]](#ref1), o uso desse diagrama contribui diretamente para o levantamento e a organização dos requisitos funcionais, servindo como uma ferramenta essencial na comunicação entre desenvolvedores, analistas e demais stakeholders. Dessa forma, o **Diagrama de Casos de Uso** não apenas delimita o escopo do sistema, mas também auxilia na visualização das funcionalidades principais de forma simples e intuitiva.

Neste contexto, o presente artefato tem como **objetivo** apresentar o Diagrama de Casos de Uso do WebApp Carona Amiga FCTE, evidenciando as interações entre os motoristas e passageiros e as funcionalidades disponibilizadas pelo sistema.

## Objetivos

Com o propósito de demonstrar as funcionalidades da plataforma sob a perspectiva dos usuários e sistemas externos, este documento busca:

- Representar as principais funcionalidades do sistema de forma visual e compreensível;
- Identificar os atores envolvidos e suas respectivas interações com a plataforma;
- Delimitar o escopo funcional do WebApp entre os envolvidos no desenvolvimento do sistema por meio de uma visão geral estruturada.

## Metodologia

Para a construção do diagrama, Serão seguidas as etapas abaixo:

1.  Serão analisados os seguintes artefatos para identificação de atores, funcionalidades e escopo:
    - [Requisitos Funcionais e Não Funcionais elicitados - Elaborados na entrega 1](../Modelagem/2.5.IniciativasExtras/RequisitosElicitados.md);
    - [Diagrama de Classe](../Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md);
    - [Diagrama de Comunicação](../Modelagem/2.2.ModelagemDinamica/Diagrama_de_comunicacao.md);
    - [BrainStorming realizado na entrega 1](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/2-Artefato-Generalista/Brainstorm).
     - [Protótipo realizado na entrega 1](https://unbarqdsw2026-1-turma02.github.io/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/#/Base/1-Design-Sprint/Prototipo).

2.  Após a análise dos dados, serão feitas as seguintes etapas:
    1. Identificação dos Atores principais.
    2. Identificação dos Casos de Uso essenciais a partir dos requisitos funcionais.
    3.  Identificação dos Relacionamentos entre Atores e Casos de Uso (Associação) e entre Atores (Generalização).
    4.  Modelagem do diagrama utilizando a ferramenta Draw.io.
    5. Verificação do diagrama por meio de revisão entre os membros do grupo, garantindo a coerência e a clareza das informações representadas.
    6. Documentação do diagrama, explicando os elementos e as interações representadas, para facilitar a compreensão por parte de todos os envolvidos no projeto.

    ## Sobre o Diagrama de Casos de Uso

> <a name="ref1"></a>**[1]** Creately. *Tutorial do diagrama de caso de uso (guia com exemplos)*. Disponível em: <https://creately.com/blog/pt/diagrama/tutorial-de-diagrama-de-caso-de-uso/>. Acesso em: 22 abr. 2026.
O Diagrama de Casos de Uso a seguir, na figura 2, elaborado com base nos princípios da UML de [Tutorial do diagrama de caso de uso (guia com exemplos)](), representa as principais interações funcionais da plataforma "Galáxia Conectada". Dessa maneira, ele destaca os `Atores` chave, como `Motorista`, `Passageiro` e sistemas como `Serviços de Autenticação`, `Sistema de Notificação`. Além disso, os `Casos de Uso` (elipses) representam as funcionalidades do sistemas, como realizar login, aceita/cancelar carona, entre outros.

Para compreensão dos diagramas, a figura 1 mostra a legenda;

<font size="3"><p style="text-align: center">Figura 1: Legenda do Diagrama de Casos de Uso</p></font>


<div align="center">
    <img src="https://i.postimg.cc/fZxMGrPC/legenda-uml.png" width="500">
</div>

<font size="2"><p style="text-align: center">Fonte: [Luiza da Silva Pugas](https://github.com/luizaxx), 2026.</p></font>

## Diagrama de Casos de Uso

A Figura 2 mostra o diagrama de Casos de Uso do WebApp Carona Amiga FCTE. 

<font size="3"><p style="text-align: center">Figura 2: Diagrama de Casos de Uso</p></font>

<div align="center">
    <img src="../docs/assets/diagrama_casos_uso/Casos%20de%20uso.png" width="1000">
</div>

<font size="2"><p style="text-align: center">Fonte: Elaborado pelo(s) autor(es): [Ana Victória Guedes da Costa](https://github.com/navicg), [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Karoline Luz da Conceição](https://github.com/KarolineLuz), [Luiza da Silva Pugas](https://github.com/Luizaxx) e
[Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), 2026.</p></font>

**Observação:** Caso deseje visualizar ou baixar em PDF, clique aqui:  
[PDF do Diagrama de Casos de Uso](https://drive.google.com/file/d/1-OdkNTwh7X30XgMHm83Kl2MdM_VpxkS9/view?usp=sharing)

## Conclusão
O Diagrama de Casos de Uso do WebApp Carona Amiga FCTE, apresentado na figura 2, oferece uma visão clara e estruturada das funcionalidades principais do sistema, bem como das interações entre os atores envolvidos. Através da identificação dos casos de uso essenciais, foi possível delimitar o escopo funcional do sistema, facilitando a comunicação entre os membros da equipe e demais stakeholders. Este artefato serve como um guia visual para o desenvolvimento do sistema, garantindo que as funcionalidades sejam implementadas de acordo com as necessidades dos usuários e os requisitos elicitados.

---

## Bibliografia

> <a name="ref1"></a>**[1]** Creately. *Tutorial do diagrama de caso de uso (guia com exemplos)*. Disponível em: <https://creately.com/blog/pt/diagrama/tutorial-de-diagrama-de-caso-de-uso/>. Acesso em: 22 abr. 2026.

> <a name="ref2"></a>**[2]** DevMedia. *O que é UML e Diagramas de Caso de Uso: Introdução Prática à UML*. Disponível em: <https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408>. Acesso em: 22 abr. 2026.

> <a name="ref3"></a>**[3]** Lucidchart. *Diagrama de caso de uso UML: O que é, como fazer e exemplos*. Disponível em: <https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml>. Acesso em: 22 abr. 2026.

> <a name="ref4"></a>**[4]** Lucid Software (YouTube). *Tutorial de Caso de Uso UML - Lucid Software Português*. Disponível em: <https://www.youtube.com/watch?v=ab6eDdwS3rA>. Acesso em: 22 abr. 2026.

> <a name="ref5"></a>**[5]** Microsoft. *Criar um diagrama de caso de uso UML*. Disponível em: <https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298>. Acesso em: 22 abr. 2026.

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 23/04/2026 | Criação do documento [#10](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_02/issues/10) | [Luiza da S. Pugas](https://github.com/Luizaxx) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS)  |  |
| 1.1  | 23/04/2026 | Adição do png e pdf do diagrama de casos de uso [#10](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_02/issues/10) |[Ana Victória Guedes da Costa](https://github.com/navicg) | [Karoline Luz da Conceição](https://github.com/KarolineLuz) |  |
