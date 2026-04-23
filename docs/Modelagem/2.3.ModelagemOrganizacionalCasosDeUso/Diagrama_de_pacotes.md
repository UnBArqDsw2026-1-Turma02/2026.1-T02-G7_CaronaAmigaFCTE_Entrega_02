# Diagrama de Pacotes

## Introdução

No contexto da Linguagem de Modelagem Unificada (UML), o Diagrama de Pacotes é classificado como um diagrama estrutural responsável por representar a organização modular de um sistema por meio do agrupamento lógico de elementos relacionados. Esse tipo de diagrama permite visualizar a decomposição do sistema em unidades maiores, denominadas pacotes, evidenciando as dependências e relações existentes entre esses agrupamentos <a href="#referencias-bibliograficas-1">[1]</a>.

De acordo com a UML, um pacote consiste em um mecanismo de organização que possibilita agrupar elementos modelados, como classes, interfaces e outros artefatos, com o objetivo de estruturar o modelo de forma hierárquica e facilitar sua compreensão. Além disso, o Diagrama de Pacotes permite representar dependências, importações, acessos, mesclagens e relações de generalização entre pacotes, contribuindo para a definição de uma arquitetura mais organizada e com menor acoplamento <a href="#referencias-bibliograficas-3">[3]</a>.

A utilização desse diagrama é especialmente relevante em sistemas de maior porte, nos quais a divisão em módulos ou camadas favorece a manutenção, a escalabilidade e a evolução da aplicação. A organização adequada dos pacotes auxilia na separação de responsabilidades, promovendo maior clareza estrutural e alinhamento com princípios arquiteturais consolidados <a href="#referencias-bibliograficas-2">[2]</a>.

No contexto do projeto **Carona Amiga FCTE**, o Diagrama de Pacotes tem como finalidade representar a organização estrutural do sistema em nível macro, demonstrando como seus elementos estão agrupados e como se relacionam entre si. Dessa forma, o artefato contribui para a compreensão global da arquitetura proposta e para a validação da coerência entre os diferentes módulos que compõem a solução.

---

## Objetivos

Com base na elaboração do Diagrama de Pacotes para o projeto **Carona Amiga FCTE**, têm-se como objetivos:

- Representar a organização modular do sistema por meio do agrupamento lógico de seus elementos.
- Identificar e estruturar pacotes de acordo com responsabilidades funcionais e arquiteturais.
- Evidenciar as dependências existentes entre os pacotes do sistema.
- Demonstrar a direção das relações de dependência, promovendo maior controle do acoplamento.
- Auxiliar na visualização da arquitetura em alto nível da aplicação.
- Contribuir para a coerência entre o Diagrama de Classes e a organização estrutural proposta.

---

## Metodologia

A elaboração do Diagrama de Pacotes do projeto **Carona Amiga FCTE** será conduzida com base nos princípios da UML e nas boas práticas de modularização de sistemas, buscando representar de forma clara a organização estrutural da aplicação.

Inicialmente, será realizada uma análise dos artefatos previamente desenvolvidos pela equipe, com o objetivo de identificar agrupamentos lógicos coerentes entre classes, componentes e funcionalidades do sistema. Essa análise terá como base:

- [Projeto](/Projeto/Projeto.md);
- [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md);
- [Diagrama de Casos de Uso](/Modelagem/2.2.ModelagemComportamental/Diagrama_de_casos_de_uso.md).

A partir dessa análise, serão definidos os pacotes do sistema, considerando critérios como responsabilidade funcional, separação de interesses, coesão interna e baixo acoplamento entre módulos. Em seguida, serão identificadas as dependências entre os pacotes, observando a direção das relações e sua aderência à arquitetura pretendida.

Após a definição da estrutura inicial, o diagrama será construído em ferramenta apropriada de modelagem, respeitando a notação padronizada da UML para pacotes, dependências e estereótipos. Por fim, o artefato passará por uma etapa de verificação, garantindo sua consistência com os demais modelos estruturais e comportamentais do projeto.

---

## Modelagem

A modelagem do Diagrama de Pacotes do projeto **Carona Amiga FCTE** foi realizada com o objetivo de representar a organização estrutural do sistema em nível macro. O diagrama evidencia os principais agrupamentos definidos, bem como as dependências existentes entre eles.

Os pacotes foram organizados considerando critérios arquiteturais e de separação de responsabilidades, permitindo maior modularidade e clareza estrutural. As relações de dependência demonstram como determinados módulos utilizam funcionalidades ou elementos definidos em outros pacotes, reforçando a necessidade de controle do acoplamento.

A representação segue a notação UML, na qual cada pacote é identificado por um retângulo com aba superior, contendo o nome do agrupamento. As dependências são indicadas por setas tracejadas, podendo apresentar estereótipos específicos conforme o tipo de relação estabelecida.

---

## Tabela de Análise

| Componente / Notação               | Representação                  | Descrição                                                                                                                   |
| ---------------------------------- | ------------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| **Pacote**                         | Retângulo com aba superior     | Representa um agrupador lógico utilizado para organizar elementos do sistema, como classes, casos de uso ou outros pacotes. |
| **Elemento Contido**               | Elementos internos ao pacote   | Indica componentes pertencentes ao pacote, podendo possuir níveis de visibilidade definidos.                                |
| **Dependência** (`<<dependency>>`) | Seta tracejada                 | Demonstra que um pacote depende de outro, podendo sofrer impacto em caso de modificações no fornecedor.                     |
| **Importação** (`<<import>>`)      | Seta tracejada com estereótipo | Permite que elementos públicos de um pacote sejam utilizados diretamente por outro.                                         |
| **Acesso** (`<<access>>`)          | Seta tracejada com estereótipo | Concede acesso controlado aos elementos de outro pacote.                                                                    |
| **Mesclagem** (`<<merge>>`)        | Seta tracejada com estereótipo | Indica combinação de conteúdos entre pacotes.                                                                               |
| **Generalização**                  | Seta com triângulo vazio       | Representa herança entre pacotes, indicando especialização.                                                                 |

---

## Legenda do Diagrama

<div style="text-align: center;">
Legenda do Diagrama de Pacotes  
<br>
<img src="https://i.postimg.cc/MKqQ686k/Captura-de-tela-2026-04-23-101821.png" alt="Figura 01">
<font size="2"><p style="text-align: center">Figura 01.</p></font>
</div>

<font size="2"><p style="text-align: center">Fonte: [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) e [João Vitor Santos de Oliveira](https://github.com/Jauzimm), 2026.</p></font>

---

## Diagrama de Pacotes

<div style="text-align: center;">
Diagrama de Pacotes  
<br>
<img src="https://i.postimg.cc/BLQ1hxY6/diagramaPacotes.png" alt="Figura 02">
<font size="2"><p style="text-align: center">Figura 02.</p></font>
</div>

<font size="2"><p style="text-align: center">Fonte: [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess), [João Vitor Santos de Oliveira](https://github.com/Jauzimm), [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) e [Pedro Henrique Faria da Mota](https://github.com/PhFariaa), 2026.</p></font>

---

## Conclusão

A construção do Diagrama de Pacotes do projeto **Carona Amiga FCTE** possibilita representar de forma estruturada a organização modular do sistema, evidenciando a divisão lógica de responsabilidades e as dependências existentes entre os diferentes agrupamentos.

A divisão em pacotes facilita o entendimento da arquitetura, melhora a separação de responsabilidades e contribui para a manutenção e evolução do sistema. Em projetos de maior complexidade, essa organização torna-se essencial para garantir escalabilidade e reduzir o acoplamento entre módulos.

Além disso, o artefato fortalece a coerência entre os modelos produzidos, especialmente o Diagrama de Classes, ao demonstrar como os elementos modelados estão organizados em módulos maiores. Dessa forma, o Diagrama de Pacotes atua como instrumento fundamental para apoiar decisões arquiteturais e promover maior clareza na comunicação entre os membros da equipe.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> LUCID SOFTWARE INC. **Diagrama de Pacotes UML**. Disponível em: https://www.lucidchart.com/pages/pt/diagrama-de-pacotes-uml. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> FAG – FACULDADE ASSIS GURGACZ. **Anais 2022 – Modelagem UML aplicada**. Disponível em: https://www4.fag.edu.br/anais-2022/Anais-2022-106.pdf. Acesso em: 23 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> UML-DIAGRAMS. **UML Package Diagrams Overview**. Disponível em: https://www.uml-diagrams.org/package-diagrams-overview.html. Acesso em: 23 abr. 2026.

> SERRANO, Milene. Slides – Diagrama de Pacotes. Universidade de Brasília.

---

## Histórico de Versões

| Versão | Data       | Descrição                                                   | Autor(es)                                                                                                                     | Revisor(es)                                                  | Detalhes da Revisão |
| :----: | ---------- | ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ | ------------------- |
|  1.0   | 20/04/2026 | Criação inicial da seção de diagrama de pacotes             | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) e [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | Artefato revisado   |
|  1.1   | 21/04/2026 | Inserção do diagrama e estruturação do conteúdo             | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) e [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | Artefato revisado   |
|  1.2   | 22/04/2026 | Ajustes na explicação e melhoria da descrição dos elementos | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) e [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | Artefato revisado   |
|  1.3   | 23/04/2026 | Revisão final e padronização do documento                   | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) e [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) | [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk) | Artefato revisado   |
|  2.0   | 23/04/2026 | Integração ao padrão estrutural do projeto                  | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima)                                                        |                                                              |                     |
|  2.1   | 23/04/2026 | Ajustes e consolidação das referências                      | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima)                                                        |                                                              |                     |
|  2.1   | 23/04/2026 | Ajustes dos links nas fontes                                | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima)                                                        |                                                              |                     |
