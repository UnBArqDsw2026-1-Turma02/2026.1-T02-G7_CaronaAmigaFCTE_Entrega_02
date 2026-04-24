# Verificação do Diagrama de Classes

## Introdução

Ao considerar a Apostila UML [[1]](#ref1), o Diagrama de Classes é um dos elementos centrais da modelagem estática em UML, usado para representar a estrutura de um sistema por meio de suas classes, atributos, métodos e relacionamentos. Sendo assim, no projeto da Carona Amiga FCTE, esse diagrama foi elaborado para modelar as entidades principais do sistema. 

A validação e a verificação do Diagrama de Classes são etapas cruciais para garantir que o modelo esteja correto, completo e consistente com os requisitos do sistema. A validação é o processo de assegurar que o diagrama representa fielmente os requisitos e as necessidades do sistema, enquanto a verificação é o processo de avaliar se o diagrama foi construído corretamente, conforme os critérios da UML. A seguir, serão detalhados os processos de validação e verificação do Diagrama de Classes, destacando a importância de cada etapa para o desenvolvimento de um sistema.

## Objetivo da Verificação

O objetivo da verificação do Diagrama de Classes é garantir que o modelo esteja correto, completo e consistente com os requisitos do sistema. Isso envolve a identificação de erros, inconsistências e omissões no diagrama, bem como a validação de que ele representa adequadamente as entidades e os relacionamentos do sistema. A verificação é essencial para evitar problemas futuros durante a implementação e manutenção do sistema, garantindo que o modelo seja uma representação precisa da realidade do domínio do problema.

## Metodologia de Verificação

A metodologia de verificação do Diagrama de Classes envolve as seguintes etapas:
1. **Revisão de Requisitos**: Verificar se o diagrama de classes está alinhado com os requisitos do sistema, garantindo que todas as entidades e relacionamentos necessários estejam representados.
2. **Análise de Consistência**: Avaliar se o diagrama é consistente internamente, verificando se as classes, atributos e métodos estão corretamente definidos e relacionados.
3. **Identificação de Erros**: Procurar por erros comuns, como classes sem atributos ou métodos, relacionamentos incorretos ou ausentes, e inconsistências na nomenclatura.

Com essa metodologia, criamos perguntas baseadas nas referências bibliográficas para guiar a verificação do Diagrama de Classes, depois gravamos em conjunto para validar o diagrama e corrigir possíveis erros antes da entrega final.


## Tabela de Verificação do Diagrama de Classes

<font size="3"><p style="text-align: center">Tabela 1: Verificação do Diagrama de Classes</p></font>

| ID   | Pergunta de Verificação                                                                 | Verificado                                                                 | Rastreabilidade |
|------|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|-----------------|
| 01  | O nome da classe foi iniciado com letra maiúscula conforme o padrão de nomenclatura?   | Verificado                                                                  | [Webel IT Australia](https://www.webel.com.au/node/669) |
| 02  | A representação da classe contém os três compartimentos básicos (nome, atributos e métodos)? | Verificado                                                                  | Apostila UML, seção sobre representação de classes |
| 03  | O nome atribuído à classe corresponde a um substantivo que represente uma entidade?    | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
| 04  | Os atributos estão descritos com identificação clara e seus respectivos tipos?         | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
| 05  | As operações da classe estão especificadas com nomes e parâmetros definidos?           | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
|   06  | A classe modela uma entidade importante dentro do contexto do sistema?                 | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
| 07  | Foram consideradas e incluídas classes externas (como bibliotecas ou sistemas integrados)? | Verificado                                                                  | Apostila UML, seção sobre bibliotecas e sistemas externos |
| 08  | Existe relação da classe com algum ator do sistema (ex: usuário, administrador)?       | Verificado                                                                  | Apostila UML, seção sobre papéis de atores |
| 09  | Os nomes dos atributos seguem o padrão camelCase?                                      | Verificado                                                                  | [Ez Knowledge](https://www.ez-knowledge.com/comprehensive-guide-to-uml-class-diagrams/) |
| 10  | Os nomes dos métodos utilizam a convenção camelCase?                                   | Verificado                                                                  | [Ez Knowledge](https://www.ez-knowledge.com/comprehensive-guide-to-uml-class-diagrams/) |
| 11  | A formatação dos atributos e métodos está padronizada (alinhamento à esquerda e fonte comum)? | Verificado                                                                  | [UML Diagrams](https://www.uml-diagrams.org/class-reference.html) |
| 12  | Todos os métodos apresentam parênteses, mesmo quando não possuem parâmetros?           | Verificado                                                                  | [University of Cape Town](https://www.cs.uct.ac.za/mit_notes/software/htmls/ch05s09.html) |
| 13  | Os atributos e métodos estão organizados considerando níveis de visibilidade (do mais visível ao menos visível)? | Verificado                                                                  | [Creately Blog](https://creately.com/blog/diagrams/guidelines-for-uml-class-diagrams-part-1/) |
| 14  | Os nomes dos métodos utilizam verbos no infinitivo para indicar ações?                 | Verificado                                                                  | [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-class-diagram-tutorial/) |
| 15  | Os métodos apresentam seus parâmetros acompanhados dos respectivos tipos?             | Verificado                                                                  | [UML Diagrams](https://www.uml-diagrams.org/class-reference.html) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva Pugas](https://github.com/luizaxx) e [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), 2026.</p></font>

---

## Verificação de Relacionamentos no Diagrama de Classes

<font size="3"><p style="text-align: center">Tabela 2: Verificação dos Relacionamentos no Diagrama de Classes</p></font>

| ID   | Pergunta de Verificação                                                                 | Verificado                                                                  | Rastreabilidade |
|------|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|-----------------|
| 01 | As ligações entre classes foram desenhadas com linhas contínuas e possuem indicação de direção quando necessário? | Verificado                                                                  | Apostila UML; [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
| 02 | As cardinalidades (como 1..*, 0..1) estão corretamente definidas nas associações?       | Verificado                                                                  | Apostila UML; [Creately](https://creately.com/blog/diagrams/guidelines-for-uml-class-diagrams-part-1/) |
| 03 | As relações de dependência estão representadas com linhas tracejadas e setas apontando para a classe dependida? | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |
| 04 | As heranças foram representadas com linhas contínuas e seta de triângulo vazio direcionada à superclasse? | Verificado                                                                  | Apostila UML; [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-class-diagram-tutorial/) |
| 05 | As relações de agregação estão indicadas com losango vazio na classe que representa o todo? | Verificado                                                                  | [TutorialsPoint](https://www.tutorialspoint.com/uml/uml_aggregation.htm) |
| 06 | As composições estão corretamente ilustradas com losango preenchido na extremidade da classe composta? | Verificado                                                                  | [Visual Paradigm](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-class-diagram-tutorial/) |
| 07 | As associações em que a classe se relaciona consigo mesma estão corretamente representadas? | Verificado                                                                  | [Guru99](https://www.guru99.com/uml-class-diagram.html) |
| 08 | As implementações de interfaces estão indicadas com linha tracejada e seta com triângulo vazio apontando para a interface? | Verificado                                                                  | [GeeksforGeeks](https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva Pugas](https://github.com/luizaxx) e [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), 2026.</p></font>

---

## Vídeo de Verificação do Diagrama de Classes
O vídeo de verificação do Diagrama de Classes foi gravado para validar o modelo criado, utilizando as perguntas de verificação como guia para identificar possíveis erros e inconsistências. Durante a gravação, foram discutidos os pontos fortes do diagrama, bem como as áreas que necessitavam de ajustes.

<iframe width="1321" height="743" src="https://www.youtube.com/embed/lEFFf72zMhw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/lEFFf72zMhw" target="_blank">Clique aqui para assistir no YouTube</a></p>

<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva Pugas](https://github.com/luizaxx) e [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), 2026.</p></font>

---

## Conclusão
A verificação do Diagrama de Classes é um processo fundamental para garantir a qualidade e a eficácia do modelo de um sistema. Ao seguir uma metodologia estruturada de verificação, é possível identificar e corrigir erros, inconsistências e omissões no diagrama, garantindo que ele seja uma representação precisa e útil do sistema. A validação com stakeholders é especialmente importante para garantir que o modelo atenda às necessidades do sistema e seja compreendido por todos os envolvidos no projeto. Em última análise, a verificação do Diagrama de Classes contribui para o sucesso do desenvolvimento do sistema, proporcionando uma base sólida para a implementação e manutenção futura.

## Bibliografia

>  1. APOSTILA UML. Seção sobre representação de classes. Disponíbilizada pela professora. Acesso em: 23 abr. 2026.
>  2. BÓSON TREINAMENTOS. Introdução à UML – Unified Modeling Language. Disponível em: https://www.youtube.com/watch?v=C3xYBT3o_5k. Acesso em: 23 abr. 2026.
>  3. BÓSON TREINAMENTOS. Curso de UML: O que é um diagrama de Classes. Disponível em: https://www.youtube.com/watch?v=JQSsqMCVi1k. Acesso em: 23 abr. 2026.
>  4. CREATELY. Class Diagram Relationships. Disponível em: https://creately.com/guides/class-diagram-relationships/. Acesso em: 23 abr. 2026.
>  5. EZ KNOWLEDGE. Comprehensive Guide to UML Class Diagrams. Disponível em: https://www.ez-knowledge.com/comprehensive-guide-to-uml-class-diagrams/. Acesso em: 23 abr. 2026.
>  6. GEEKSFORGEEKS. Unified Modeling Language (UML) Class Diagrams. Disponível em: https://www.geeksforgeeks.org/unified-modeling-language-uml-class-diagrams/. Acesso em: 23 abr. 2026.
>  7. GURU99. UML Relationships with Example. Disponível em: https://www.guru99.com/uml-relationships-with-example.html. Acesso em: 23 abr. 2026.
>  8. TUTORIALSPOINT. UML Association vs Aggregation vs Composition. Disponível em: https://www.tutorialspoint.com/uml/uml_association_vs_aggregation_vs_composition.htm. Acesso em: 25 abr. 2026.
>  9. UML DIAGRAMS. Class Reference. Disponível em: https://www.uml-diagrams.org/class-reference.html. Acesso em: 23 abr. 2026.
>  10. UML DIAGRAMS. Class Diagrams Overview. Disponível em: https://www.uml-diagrams.org/class-diagrams-overview.html. Acesso em: 23 abr. 2026.
>  11. UNIVERSITY OF CAPE TOWN. Software Engineering Notes. Disponível em: https://www.cs.uct.ac.za/mit_notes/software/htmls/ch05s09.html. Acesso em: 23 abr. 2026.
>  12. VISUAL PARADIGM. UML Aggregation vs Composition. Disponível em: https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-aggregation-vs-composition/. Acesso em: 25 abr. 2026.
>  13. WEBEL IT AUSTRALIA. UML Class Diagrams. Disponível em: https://www.webel.com.au/node/669. Acesso em: 23 abr. 2026.

## Histórico de Versões

| Versão |    Data    | Descrição                                                                                                                                                                                                    | Autor(es)                                                              | Revisor(es)                                                       | Detalhes da revisão |
| :----: | :--------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------- | ----------------------------------------------------------------- | :-----------------: |
|  1.0   | 23/04/2026 | Criação do artefato e elaboração da tabela de verificação | [Luiza da Silva Pugas](https://github.com/Luizaxx) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Estrutura inicial do documento e checklist de verificação |
|  1.1   | 23/04/2026 | Arrumando os links e adicionando os nomes | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Verificação dos links e nomes dos videos e corrigindo ordem |