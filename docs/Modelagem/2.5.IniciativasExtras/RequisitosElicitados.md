# Requisitos Elicitados

## Requisitos Funcionais

###  Tabela 1: Geral de Requisitos Funcionais

#### Tabela de Requisitos Funcionais (RF)

#### Consolidado

| Código | Requisito Funcional | Objetivo | Rastreabilidade |
| :--: | :-- | :-- | :-- |
| <a id="rf01-perfil"></a>RF01 (Benchmarking) / RF03 (Brainstorming) / RF21 (Brainstorming) | Gerenciar perfil do usuário (visualizar/editar). | Aumentar confiança, personalização e apoiar decisão mais segura. | Benchmarking; Brainstorming |
| <a id="rf01-cadastro"></a>RF01 (Brainstorming) | Cadastrar usuário. | Aumentar a confiança entre motorista e passageiro. | Brainstorming |
| <a id="rf02-oferta"></a>RF02 (Benchmarking) / RF08 (Brainstorming) | Criar/Publicar oferta de carona. | Estruturar e publicar ofertas com informações mínimas para decisão e atender demandas imediatas. | Benchmarking; Brainstorming |
| <a id="rf03-busca"></a>RF03 (Benchmarking) | Buscar caronas. | Melhorar precisão no encontro entre oferta e demanda. | Benchmarking |
| <a id="rf04-eta"></a>RF04 (Benchmarking) | Calcular ETA. | Apoiar planejamento e previsibilidade da viagem. | Benchmarking |
| <a id="rf14-rotas"></a>RF14 (Brainstorming) | Sugerir melhores rotas. | Reduzir tempo de deslocamento e atrasos. | Brainstorming |
| <a id="rf05-msg"></a>RF05 (Benchmarking) / RF06 (Brainstorming) | Enviar mensagem. | Facilitar comunicação e alinhamentos antes e durante a viagem. | Benchmarking; Brainstorming |
| <a id="rf06-solicitar"></a>RF06 (Benchmarking) | Solicitar participação. | Dar controle ao motorista e transparência ao passageiro. | Benchmarking |
| <a id="rf07-cancelar"></a>RF07 (Benchmarking) | Cancelar solicitação. | Reduzir ruídos e melhorar rastreabilidade de ocorrências. | Benchmarking |
| <a id="rf08-avaliar"></a>RF08 (Benchmarking) / RF04 (Brainstorming) | Avaliar viagens/experiência. | Construir reputação e melhorar a qualidade das caronas/comunidade. | Benchmarking; Brainstorming |
| <a id="rf09-bloquear"></a>RF09 (Benchmarking) | Bloquear usuário. | Reforçar segurança e moderação da plataforma. | Benchmarking |
| <a id="rf10-notificacoes"></a>RF10 (Benchmarking) / RF09 (Brainstorming) | Enviar notificações (caronas). | Aumentar pontualidade e chance de correspondência entre oferta e demanda. | Benchmarking; Brainstorming |
| <a id="rf05-favoritar"></a>RF05 (Brainstorming) | Favoritar motoristas. | Facilitar recorrência de caronas confiáveis. | Brainstorming |
| <a id="rf07-grupo"></a>RF07 (Brainstorming) | Criar grupo de carona. | Viabilizar caronas fixas na semana. | Brainstorming |
| <a id="rf10-grade"></a>RF10 (Brainstorming) | Gerar grade horária de caronas. | Facilitar planejamento de ida e volta. | Brainstorming |
| <a id="rf13-mapa"></a>RF13 (Brainstorming) | Gerar mapa com caronas. | Melhorar visualização espacial das opções. | Brainstorming |
| <a id="rf17-localizacao"></a>RF17 (Brainstorming) | Compartilhar localização. | Aumentar rastreabilidade e segurança. | Brainstorming |
| <a id="rf18-desvio"></a>RF18 (Brainstorming) | Detectar desvio da rota. | Reagir rapidamente a situações de risco. | Brainstorming |
| <a id="rf19-contatos"></a>RF19 (Brainstorming) | Notificar contatos. | Oferecer resposta imediata em incidentes. | Brainstorming |
| <a id="rf20-embarque"></a>RF20 (Brainstorming) | Validar embarque. | Confirmar identidade e evitar fraudes. | Brainstorming |
| <a id="rf24-historico"></a>RF24 (Brainstorming) | Registrar histórico. | Permitir auditoria, consulta e transparência para o usuário. | Brainstorming |
| <a id="rf25-recomendacao"></a>RF25 (Brainstorming) | Recomendar caronas. | Melhorar pontualidade e aderência às necessidades do usuário. | Brainstorming |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>



##  Requisitos Não Funcionais

###  Tabela 2: Geral de Requisitos Não Funcionais


#### Consolidado

| Código | Categoria FURPS+ | Requisito Não Funcional | Objetivo | Rastreabilidade |
| :--: | :--: | :-- | :-- | :-- |
| RNF01 | Usabilidade (U) | O sistema deve ser responsivo para desktop, tablet e mobile. | Garantir boa usabilidade e uso consistente em diferentes dispositivos. | Benchmarking; Brainstorming |
| RNF02 (Benchmarking) | Suportabilidade (S) | O sistema deve proteger dados sensíveis com boas práticas de segurança (hash de senha, TLS e controle de acesso). | Preservar privacidade e integridade das contas. | Benchmarking |
| RNF02 (Brainstorming) | Performance (P) | O sistema deve responder em menos de 2 segundos nas operações principais (buscar carona, publicar carona e abrir mapa), medido em p90. | Manter navegação fluida para passageiros e motoristas. | Brainstorming |
| RNF03 (Benchmarking) / RNF06 (Brainstorming) | Usabilidade (U) | O sistema deve ter fluxo simples e linguagem clara para ações centrais, com validação por testes de usabilidade. | Reduzir fricção de uso e curva de aprendizado para novos usuários. | Benchmarking; Brainstorming |
| RNF04 (Benchmarking) / RNF13 (Brainstorming) | Confiabilidade (R) | O sistema deve registrar logs e trilhas de auditoria de ações relevantes (ex.: aceites, cancelamentos, denúncias, cadastro, avaliação e alteração de perfil), com carimbo de data/hora e retenção definida. | Aumentar auditabilidade, rastreabilidade e suporte a incidentes. | Benchmarking; Brainstorming |
| RNF04 (Brainstorming) | Confiabilidade (R) | O sistema deve manter disponibilidade mensal mínima de 99,5%, com monitoramento de uptime, alertas automáticos e plano de contingência para indisponibilidade. | Evitar interrupções no uso diário da plataforma. | Brainstorming |
| RNF05 (Brainstorming) | Usabilidade (U) | O sistema deve atender à acessibilidade conforme WCAG 2.1 nível AA, incluindo contraste adequado, navegação por teclado, textos alternativos e suporte a leitores de tela. | Incluir pessoas com deficiência no uso da plataforma. | Brainstorming |
| RNF06 (Benchmarking) | Performance (P) | O sistema deve apresentar rotas e estimativas de tempo de forma consistente. | Melhorar previsibilidade da experiência de deslocamento. | Benchmarking |
| RNF07 (Brainstorming) | Performance (P) | O sistema deve suportar aumento gradual de usuários por meio de escalabilidade horizontal e cache, mantendo tempo de resposta dentro da meta sob carga concorrente definida. | Preservar desempenho durante crescimento da base de usuários. | Brainstorming |
| RNF09 (Brainstorming) | Suportabilidade (S) | O sistema deve funcionar nas duas últimas versões estáveis de Chrome, Firefox, Edge e Safari, com testes de compatibilidade a cada release. | Assegurar acesso para a maioria dos usuários em navegadores modernos. | Brainstorming |
| RNF10 (Brainstorming) | Performance (P) | O sistema deve operar com internet limitada utilizando carregamento progressivo, compressão de recursos e fallback para modo de baixo consumo de dados em rede 3G/4G instável. | Manter acesso para usuários em conexões lentas ou instáveis. | Brainstorming |
| RNF11 (Brainstorming) | Performance (P) | O sistema deve entregar notificações críticas (emergência e desvio de rota) com latência de até 5 segundos após o evento, com retentativas automáticas de envio. | Permitir reação rápida em situações urgentes de segurança. | Brainstorming |
| RNF12 (Brainstorming) | Restrições legais/técnicas (+) | O sistema deve coletar localização e gravações somente com consentimento explícito, registrar finalidade de uso e permitir revogação pelo usuário em conformidade com a LGPD. | Preservar privacidade e conformidade regulatória para motorista e passageiro. | Brainstorming |

<font size="2"><p style="text-align: center">Fonte: [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>