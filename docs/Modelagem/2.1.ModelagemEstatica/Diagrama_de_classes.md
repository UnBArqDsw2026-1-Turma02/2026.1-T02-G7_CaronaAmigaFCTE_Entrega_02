# Diagrama de Classes

# Introdução
Parafraseando e traduzindo o artigo [artigo da plataforma UML Diagrams](https://www.uml-diagrams.org/class-diagrams-overview.html) um diagrama de classes é um diagrama estrutural da UML que mostra a estrutura do sistema projetado no nível de **classes** e **interfaces**, exibindo seus recursos, **restrições** e **relacionamentos** — como associações, generalizações, dependências, etc.

### Tipos Comuns de Diagramas de Classes
* **Diagrama de modelo de domínio:** foca nos conceitos e regras de negócio.
* **Diagrama de classes de implementação:** foca nos detalhes técnicos e na codificação.

No prjeto Carona Amiga, um web app para conectar motoristas e passageiros, o diagrama de classes será usado para modelar os principais elementos do sistema, como usuários, caronas, veículos, etc., e suas interações com fim de organizar e compreender a estrutura do sistema (modelo de domínio). 

## Objetivos

O objetivo desse artefato é representar de forma estruturada os principais elementos do sistema Carona Amiga, suas características e relacionamentos, para facilitar a comunicação entre os membros da equipe e orientar o desenvolvimento do projeto.
 Sendo assim, as metas principais desse artefato são:

 - Apresentar o Diagrama de Classes do web app Carona Amiga, destacando as principais classes, atributos, métodos e relacionamentos;

- Documentar a arquitetura lógica do sistema;

- Fornecer uma base sólida para o desenvolvimento e manutenção do sistema;

- Servir como referência para validação dos requisitos elicitados;

## Metodologia

1.  <img src="https://store-images.s-microsoft.com/image/apps.1409.13851527096222888.2b60149a-04a5-4578-a6b2-d7b7377332d5.c22d8e97-4d44-4304-9bd2-55f9d29c0f82?h=210" width="25" height="25" align="center">  O **Diagrama de Classes** será desenvolvido utilizando a ferramenta [Draw.io](https://app.diagrams.net/), a qual permite a criação de diagramas UML de forma prática e visual.

2. Como base para a definição das classes, serão utilizadas as informações coletadas na [Entrega 01 do projeto](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01), a qual inclui:

- **Requisitos Funcionais:** para identificar as funcionalidades que o sistema deve oferecer e, consequentemente, as classes necessárias para implementá-las. [Requisitos funcionais](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md#rf01);

- **Requisitos Não Funcionais:** para considerar aspectos como desempenho, segurança, usabilidade, etc., que podem influenciar a estrutura do sistema e as classes envolvidas.
[Requisitos não funcionais](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/MoSCoW.md#rf01);

Informações adicionais, como [5W2H](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/5w2h.md), [Brainstorming](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/Brainstorm.md), [Benchmarking](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/Benchmarking.md) e [Personas](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/5-Iniciativas-Extras/Personas.md), também serão consideradas para garantir que o diagrama de classes reflita adequadamente as necessidades do sistema.

- **Atores do sistema:** [Atores do sistema identificados no Rich Picture](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/blob/main/docs/Base/2-Artefato-Generalista/1.3.RichPicture.md);


3. Serão definidas as classes do sistema, junto com seus atributos e métodos. Após compreender e definir bem as classes, serão analisados os relacionamentos de cada um delas. 

4. Por fim, o diagrama será elaborado e, em seguida, verificado de acordo com uma [tabela de verificação](Modelagem/2.6.VerificacaoDosDiagramas/VerificacaoDosDiagramas.md) baseada nos critérios sintáticos e semânticos da UML.

# Composição — Notação UML

| Elemento | Composição | Descrição |
|---|---|---|
| **Classe** | ![Classe](https://upload.wikimedia.org/wikipedia/commons/f/f0/Diagrama_de_Classes_com_duas_classes.png) | Representa um modelo ou tipo de objeto. |
| **Atributo** | ![Atributo](https://spaceprogrammer.com/wp-content/uploads/2017/09/notacao-de-diagrama-de-classe-3.jpg) | Características ou propriedades de uma classe. |
| **Método** | ![Método](https://spaceprogrammer.com/wp-content/uploads/2017/09/notacao-de-diagrama-de-classe-3.jpg) | Funções ou comportamentos que a classe pode executar. |
| **Associação** | `──────────────` | Relacionamento entre duas ou mais classes. |
| **Herança** | `──────────────►` | Relação onde uma classe herda atributos e métodos de outra. |
| **Agregação** | `──────────────◇` | Relacionamento onde uma classe contém outra, mas com menos dependência. |
| **Composição** | `──────────────◆` | Relacionamento mais forte onde uma classe contém outra de forma dependente. |
| **Dependência** | `- - - - - - - ►` | Indica que uma classe usa outra, mas não a possui. |
| **Visibilidade** |`┌──────────────┐`<br>`│  Classname   │`<br>`├──────────────┤`<br>`│+ field: type │`<br>`├──────────────┤`<br>`│- method(): type│`<br>`└──────────────┘`  | Define o acesso aos membros de uma classe (público, privado, protegido). |
| **Pacote** | `┌─Package──────┐`<br>`│Packaged elem1│`<br>`└──────────────┘` | Agrupa classes relacionadas. |


