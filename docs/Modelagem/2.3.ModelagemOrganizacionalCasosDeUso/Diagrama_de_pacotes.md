## 2.3.4 Diagrama de Pacotes

### 2.3.4.1 Componentes e Notação do Diagrama de Pacotes

| Componente / Notação | Símbolo / Representação | Descrição |
| :--- | :--- | :--- |
| **Pacote** | Retângulo com uma aba superior | Representa um agrupador lógico utilizado para organizar elementos do sistema, como classes, casos de uso ou outros pacotes, facilitando a modularização. |
| **Elemento Contido** | Elementos dentro do pacote | Indica componentes que pertencem ao pacote, podendo ter níveis de visibilidade definidos. |
| **Dependência** (`<<dependency>>`) | Seta tracejada | Demonstra que um pacote depende de outro, ou seja, alterações no pacote fornecedor podem impactar o cliente. |
| **Importação** (`<<import>>`) | Seta tracejada com estereótipo | Permite que elementos públicos de um pacote sejam utilizados diretamente por outro, sem necessidade de qualificação. |
| **Acesso** (`<<access>>`) | Seta tracejada com estereótipo | Concede acesso aos elementos de outro pacote, porém sem torná-los visíveis publicamente. |
| **Mesclagem** (`<<merge>>`) | Seta tracejada com estereótipo | Indica a combinação de conteúdos entre pacotes, permitindo extensão de definições existentes. |
| **Generalização** | Seta com triângulo vazio | Representa herança entre pacotes, onde um pacote especializado deriva de outro mais geral. |

### 2.3.4.2 Diagrama de Pacotes

<p align="center"> Imagem - Diagrama de Pacotes </p>

<p align="center">
<a href="https://drive.google.com/file/d/1ma8bNKbBOnufKOxqaaNZAImbfM6WdHjW/view" target="_blank">
  <img src="https://i.postimg.cc/BLQ1hxY6/diagramaPacotes.png" alt="Diagrama de Pacotes" />
</a>
</p>

<p align="center">
<b>Fonte: </b>Autoria de 
<a href="https://github.com/GustavoLinharess">Gustavo Ribeiro</a> e 
<a href="https://github.com/PhFariaa">Pedro Henrique</a>
</p>

---

## 2.3.5 Conclusão

O diagrama de pacotes é essencial para a organização estrutural do sistema, pois permite visualizar como os diferentes elementos estão distribuídos em módulos. Essa divisão facilita o entendimento da arquitetura e contribui para uma melhor separação de responsabilidades.

Além disso, a utilização de pacotes auxilia na manutenção e evolução do sistema, tornando mais escalável e organizado, principalmente em projetos de maior complexidade.

---

## 2.3.6 Referências

> SERRANO, Milene. Disponível em: [Slides - Diagrama de Pacotes](https://aprender3.unb.br/pluginfile.php/3178533/mod_page/content/1/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Modelagem%20UML%20Estática%20-%20Profa.%20Milene.pdf).

> LUCIDCHART. Diagrama de pacotes UML. Disponível em: https://www.lucidchart.com/pages/pt/uml-package-diagram.

---

## 2.3.7 Histórico de Versão

| Versão | Data       | Descrição                                                                 | Autor                                      | Revisor           |
| :----: | ---------- | ------------------------------------------------------------------------- | ------------------------------------------ | ----------------- |
|  `1.0` | 20/04/2026 | Criação inicial da seção de diagrama de pacotes                          | Gustavo Ribeiro e Pedro Henrique           | Nicolas Bomfim    |
|  `1.1` | 21/04/2026 | Inserção do diagrama e estruturação do conteúdo                          | Gustavo Ribeiro e Pedro Henrique           | Nicolas Bomfim    |
|  `1.2` | 22/04/2026 | Ajustes na explicação e melhoria da descrição dos elementos              | Gustavo Ribeiro e Pedro Henrique           | Nicolas Bomfim    |
|  `1.3` | 23/04/2026 | Revisão final e padronização do documento                                | Gustavo Ribeiro e Pedro Henrique           | Nicolas Bomfim    |