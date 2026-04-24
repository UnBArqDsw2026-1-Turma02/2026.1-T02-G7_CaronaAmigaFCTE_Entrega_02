# Verificação do Diagrama de Casos de Uso

## Introdução

De acordo com a apostila UML [1], a modelagem de um diagrama use-case é uma técnica usada para descrever e definir os requisitos funcionais de um sistema. Eles são escritos em termos de atores externos, use-
cases e o sistema modelado. Os atores representam o papel de uma entidade externa ao
sistema como um usuário, um hardware, ou outro sistema que interage com o sistema
modelado. Os atores iniciam a comunicação com o sistema através dos use-cases, onde o use-
case representa uma sequência de ações executadas pelo sistema e recebe do ator que lhe
utiliza dados tangíveis de um tipo ou formato já conhecido, e o valor de resposta da execução
de um use-case (conteúdo) também já é de um tipo conhecido, tudo isso é definido juntamente
com o use-case através de texto de documentação.

## Objetivos da Verificação
O objetivo deste artefato é verificar o diagrama de casos de uso, para isso, foram elaboradas perguntas que buscam avaliar a qualidade do diagrama, a partir de critérios como clareza, consistência, completude e aderência aos requisitos do sistema. Através dessas perguntas, é possível identificar pontos fortes e áreas de melhoria no diagrama de casos de uso, contribuindo para a construção de um modelo mais robusto e eficaz.

## Metodologia
A metodologia utilizada para a elaboração das perguntas de verificação do diagrama de casos de uso envolveu uma análise detalhada do diagrama, considerando os seguintes aspectos:
1. **Clareza**: Os atores e os casos de uso estão claramente identificados? O diagrama é fácil de entender para os stakeholders?
2. **Consistência**: O diagrama de casos de uso está consistente com outros diagramas do projeto, como o diagrama de classes e o diagrama de comunicação? 
3. **Completude**: O diagrama de casos de uso cobre todas as funcionalidades necessárias para o sistema? Existem casos de uso faltando?


Dessa forma, elaboramos uma série de perguntas que buscam avaliar a qualidade do diagrama e por fim gravamos um vídeo respondendo as perguntas elaboradas e arrumando possíveis erros encontrados.


## Tabela de Verificação do Diagrama de Casos de Uso

| ID   | Pergunta de Verificação                                                                 | Verificado | Rastreabilidade |
|------|------------------------------------------------------------------------------------------|------------|-----------------|
| 01 | O sistema está delimitado por um retângulo que representa claramente seu escopo?       | Verificado | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 02 | Todos os casos de uso estão posicionados dentro do limite do sistema?                  | Verificado | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 03 | Os atores são representados por ícones de boneco (stick figure)?                       | Verificado  | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 04 | Cada ator representa um papel (humano ou sistema externo) que interage com o sistema?  |  Verificado | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 05 | Os atores estão posicionados fora do limite do sistema?                                | Verificado  | https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298 |
| 06 | Os atores foram nomeados de forma genérica (ex: “Usuário”, “Administrador”)?           | Verificado | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 07 | O ator primário está posicionado preferencialmente à esquerda do sistema?              | Verificado  | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 08 | O ator primário inicia interações com os casos de uso?                                 | Verificado  | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 09 | Os atores secundários respondem ou dão suporte às interações do sistema?               |Verificado  | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 10 | Os casos de uso estão nomeados com verbos no infinitivo (ex: “Realizar Login”)?        |Verificado | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 11 | Cada caso de uso representa uma funcionalidade clara e independente do sistema?        | Verificado| https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 12 | As associações entre atores e casos de uso estão representadas por linhas simples?     | Verificado | https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298 |
| 13 | Os relacionamentos <<include>> estão corretamente utilizados para reutilização?        | Verificado | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 14 | Os relacionamentos <<extend>> representam comportamentos opcionais ou condicionais?    | Verificado | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 15 | As generalizações entre atores ou casos de uso estão corretamente indicadas?           |Verificado | https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298 |
| 16 | O diagrama mantém clareza e legibilidade, evitando excesso de elementos?               |Verificado  | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |
| 17 | Todos os casos de uso possuem pelo menos um ator associado?                            |Verificado  | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 18 | O diagrama cobre todas as funcionalidades principais dos requisitos do sistema?        | Verificado | https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408 |
| 19 | As interações entre atores e sistema estão consistentes com o comportamento esperado?  | Verificado  | https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298 |
| 20 | O diagrama está coerente com outros artefatos (ex: classes, comunicação)?                | Verificado   | https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml |

## Vídeo de Verificação do Diagrama de Casos de Uso

<iframe width="1321" height="743" src="https://www.youtube.com/embed/7jPwppomrm0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<p style="text-align: center"><a href="https://youtu.be/7jPwppomrm0" target="_blank">Clique aqui para assistir no YouTube</a></p>

<font size="2"><p style="text-align: center">Fonte: [Luiza da Silva Pugas](https://github.com/Luizaxx), 2026.</p></font>

## Conclusão
A verificação do diagrama de casos de uso é um processo essencial para garantir a qualidade e a eficácia do modelo de software. Através das perguntas de verificação, foi possível identificar pontos fortes e áreas de melhoria no diagrama, contribuindo para a construção de um modelo mais robusto e eficaz.

## Bibliografia
 1. APOSTILA UML. Seção sobre representação de classes. Disponíbilizada pela professora. Acesso em: 23 abr. 2026. 
 2. LUCIDCHART. Diagrama de Caso de Uso UML: Guia Completo com Exemplos. Disponível em: https://www.lucidchart.com/pages/pt/diagrama-de-caso-de-uso-uml. Acesso em: 23 de abril de 2026.
 3. DEVMEDIA. O que é UML e Diagramas de Caso de Uso? Introdução Prática à UML. Disponível em: https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408. Acesso em: 23 de abril de 2026.
 4. MICROSOFT SUPPORT. Criar um diagrama de caso de uso UML. Disponível em: https://support.microsoft.com/pt-br/topic/criar-um-diagrama-de-caso-de-uso-uml-92cc948d-fc74-466c-9457-e82d62ee1298. Acesso em: 23 de abril de 2026.

## Histórico de Versões

| Versão |    Data    | Descrição                                                                                                                                                                                                    | Autor(es)                                                              | Revisor(es)                                                       | Detalhes da revisão |
| :----: | :--------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------- | ----------------------------------------------------------------- | :-----------------: |
|  1.0   | 23/04/2026 | Criação do artefato e elaboração da tabela de verificação | [Luiza da Silva Pugas](https://github.com/Luizaxx) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Estrutura inicial do documento e checklist de verificação |
|  1.1   | 23/04/2026 | Adição do vídeo de verificação | [Ana Victória Guedes da Costa](https://github.com/navicg) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Inclusão do registro em vídeo da revisão |

