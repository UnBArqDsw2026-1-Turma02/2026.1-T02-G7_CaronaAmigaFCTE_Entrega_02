# Diagrama de Estados

## Introdução

No contexto da Linguagem de Modelagem Unificada (UML), o Diagrama de Estados, também conhecido como Diagrama de Máquina de Estados, é classificado como um diagrama comportamental responsável por representar os diferentes estados pelos quais um objeto pode passar ao longo do seu ciclo de vida, bem como os eventos que provocam transições entre esses estados. Esse tipo de diagrama é especialmente utilizado quando se deseja modelar comportamentos dinâmicos dependentes de condições, eventos e regras específicas do sistema <a href= "referencias-bibliograficas-3">[1]</a>.

De acordo com a UML, uma máquina de estados descreve como uma entidade reage a estímulos externos, alterando seu estado interno conforme eventos ocorrem. Cada estado representa uma situação estável durante a qual determinadas ações podem ser executadas, enquanto as transições indicam mudanças provocadas por eventos, podendo incluir condições de guarda e ações associadas <a href= "referencias-bibliograficas-4">[4]</a>.

Além disso, o Diagrama de Estados permite representar elementos como estado inicial, estado final, estados compostos, subestados, atividades internas e pseudoelementos de decisão, contribuindo para uma compreensão mais detalhada do comportamento do sistema em tempo de execução.

No contexto do projeto **Carona Amiga FCTE**, o Diagrama de Estados desempenha papel fundamental na modelagem do ciclo de vida dos principais elementos do sistema, permitindo visualizar de forma clara como esses elementos evoluem desde sua criação até sua finalização. Dessa forma, o artefato contribui para a validação das regras de negócio, para a identificação de possíveis inconsistências e para o alinhamento entre requisitos funcionais e comportamento esperado do sistema<a href= "referencias-bibliograficas-2">[2]</a>.

## Objetivos

Com base na elaboração do Diagrama de Estados para o projeto **Carona Amiga FCTE**, têm-se como objetivos:

- Representar o comportamento dinâmico de um elemento do sistema ao longo do seu ciclo de vida.

- Identificar os estados possíveis e as condições necessárias para a transição entre eles.

- Evidenciar eventos, ações e condições de guarda que influenciam a mudança de estados.

- Demonstrar estados iniciais e finais, bem como possíveis estados intermediários.

- Auxiliar na validação das regras de negócio definidas nos requisitos do sistema.

- Proporcionar maior clareza quanto ao fluxo comportamental do elemento modelado, contribuindo para a coerência entre os demais artefatos produzidos.

---

## Metodologia

A elaboração do Diagrama de Estados do projeto **Carona Amiga FCTE** será realizada com base nos artefatos já desenvolvidos pela equipe, buscando representar de forma consistente o comportamento dinâmico do elemento selecionado.

1. Inicialmente será realizada uma análise do material base a partir de:

- [Projeto](/Projeto/Projeto.md);
- [Diagrama de Classes](/Modelagem/2.1.ModelagemEstatica/Diagrama_de_classes.md);
- [Diagrama de Casos de Uso](/Modelagem/2.2.ModelagemComportamental/Diagrama_de_casos_de_uso.md).

2. A partir dessa análise, serão identificados:

- O estado inicial do elemento modelado;
- Os estados intermediários relevantes;
- Os eventos que provocam transições;
- As possíveis condições de guarda;
- O estado final ou situações de término do ciclo de vida.

3. Em seguida, será construída a versão inicial do diagrama na ferramenta **Miro**, contemplando estados, transições e elementos adicionais necessários à representação adequada do comportamento.

4. Após a construção, o diagrama passará por uma fase de verificação, com o objetivo de garantir sua coerência com os requisitos levantados e com os demais modelos produzidos pela equipe.

---

## Modelagem-

---

## Tabela de Análise

<div style="text-align: center;">
Legenda do Diagrama de Estados  
<br>
<img src="https://i.postimg.cc/j5Xk72Kn/image.png" alt="figura 1">
<font size="2"><p style="text-align: center">Figura 01.</p></font>
</div>
<!-- | Elemento               | Representação | Descrição                                                                                                                |
| ---------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Estado Inicial**     |               | Indica o ponto de início do ciclo de vida do elemento modelado. É representado por um círculo preenchido.                |
| **Estado**             |               | Representa uma condição ou situação na qual o objeto permanece por determinado período, podendo executar ações internas. |
| **Estado Final**       |               | Indica o término do ciclo de vida do objeto. É representado por um círculo com contorno externo.                         |
| **Transição**          |               | Representa a mudança de um estado para outro, geralmente desencadeada por um evento.                                     |
| **Evento**             |               | Fato ou ocorrência que provoca a transição entre estados.                                                                |
| **Condição de Guarda** |               | Expressão booleana que deve ser satisfeita para que a transição ocorra.                                                  |
| **Ação**               |               | Atividade executada como resultado de uma transição ou durante a permanência em um estado.                               |
| **Estado Composto**    |               | Estado que contém subestados internos, permitindo detalhamento adicional do comportamento.                               | -->

## <font size="2"><p style="text-align: center">Fonte: [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) e [João Vitor Santos de Oliveira](https://github.com/Jauzimm), 2026.</p></font>

## Diagrama de Estados

<div style="text-align: center;">
Diagrama de Estados  
<br>
<img src="" alt="figura ">
<font size="2"><p style="text-align: center">Figura 02.</p></font>
</div>

<font size="2"><p style="text-align: center">Fonte: [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) e [João Vitor Santos de Oliveira](https://github.com/Jauzimm), 2026.</p></font>

---

## Conclusão

A construção do Diagrama de Estados do projeto **Carona Amiga FCTE** permite representar de forma estruturada o comportamento dinâmico do elemento modelado, evidenciando seu ciclo de vida completo e as regras que regem sua evolução dentro do sistema. A identificação clara dos estados, eventos e transições contribui para a validação das regras de negócio e para a prevenção de ambiguidades na implementação.

Além disso, o artefato fortalece a coerência entre os requisitos definidos, o Diagrama de Classes e os demais modelos comportamentais, promovendo uma visão integrada do sistema. Dessa forma, o Diagrama de Estados atua como instrumento essencial para apoiar o desenvolvimento, a comunicação entre os membros da equipe e o entendimento global do funcionamento da plataforma **Carona Amiga FCTE**.

---

## Bibliografia

> <a id="referencias-bibliograficas-1">1.</a> LUCID SOFTWARE INC. **O que é diagrama de máquina de estados UML**. Disponível em: [https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-maquina-de-estados-uml). Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-2">2.</a> SPARX SYSTEMS. **UML 2 State Machine Diagram Tutorial**. Disponível em: [https://sparxsystems.com/resources/tutorials/uml2/state-diagram.html](https://sparxsystems.com/resources/tutorials/uml2/state-diagram.html). Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-3">3.</a> IBM CORPORATION. **State machines diagrams**. Disponível em: [https://www.ibm.com/docs/pt-br/dmrt/9.5.0?topic=diagrams-state-machines](https://www.ibm.com/docs/pt-br/dmrt/9.5.0?topic=diagrams-state-machines). Acesso em: 21 abr. 2026.

> <a id="referencias-bibliograficas-4">4.</a> UML-DIAGRAMS. **UML State Machine Diagrams**. Disponível em: [https://www.uml-diagrams.org/state-machine-diagrams.html](https://www.uml-diagrams.org/state-machine-diagrams.html). Acesso em: 21 abr. 2026.

---

## Histórico de Versões

| Versão |    Data    | Descrição                     | Autor(es)                                                              | Revisor(es)                                                 | Detalhes da revisão |
| :----: | :--------: | ----------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------- | :-----------------: |
|  1.0   | 21/04/2026 | Criação do documento          | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) |  Artefato Revisado  |
|  1.1   | 21/04/2026 | Criação do corrção dos links  | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) | [Pedro Henrique Faria da Mota](https://github.com/PhFariaa) |  Artefato Revisado  |
|  1.2   | 21/04/2026 | Adição da legenda do diagrama | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima) |                                                             |                     |
