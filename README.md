# Revolutx

Bot de inteligência artificial para Discord, mantido por **pyyrho**, com conversa contextual, recursos acadêmicos, memória, utilidades e moderação manual.

Este repositório reúne a apresentação e o guia de uso do Revolutx. O código-fonte e a hospedagem do bot são privados; esta página não distribui plugins ou uma versão para executar por conta própria.

## Módulos

### Conversa e estudo

Conversa por menção ao bot ou em canais ativados pela administração. Inclui preferências de estilo e nível acadêmico, controle de memórias, leitura de documentos e sessões de estudo. O modo acadêmico integra buscas em fontes como arXiv, Crossref, Europe PMC, OpenAlex, PubMed e Semantic Scholar; a disponibilidade depende dos serviços e das credenciais configuradas.

| Comando | Função |
| --- | --- |
| `/perfil-ia` | Define o estilo de resposta e o nível acadêmico. |
| `/memoria-ia` | Consulta o perfil, lista, registra e apaga memórias ou limpa dados de conversa. |
| `/limpar-conversa` | Apaga o histórico de conversa do usuário. |
| `/canal-ia` | Ativa ou desativa as respostas automáticas em um canal. |
| `/status-ia` | Consulta o estado dos provedores, caches e biblioteca. |
| `/diagnostico-ia` | Simula o orçamento de tokens e mostra registros de diagnóstico. |
| `/testar-ia` | Testa os modelos configurados. |
| `/limpar-cache-ia` | Limpa os caches de busca, biblioteca e respostas. |

Os comandos de canal, status, diagnóstico, teste e limpeza de cache são definidos para Administrador por padrão. As opções de memória e perfil são pessoais. Limpar a conversa e apagar memórias são ações distintas; use a opção correspondente em `/memoria-ia`.

Para iniciar uma sessão acadêmica, mencione o bot com `acadêmico iniciar [tema]`. Use as opções da sessão para continuar o trabalho. Os resultados e as referências dependem das fontes recuperadas; confira os documentos citados antes de utilizá-los em um trabalho.

### Moderação

Moderação manual com registro de avisos, notas internas, limpeza de mensagens e controle de canais. Banimentos, expulsões, silenciamentos e avisos também podem ser solicitados por menção ao bot, com verificação das permissões e da hierarquia de cargos.

| Comando | Função |
| --- | --- |
| `/config-mod` | Configura o canal de logs e o cargo de alerta. |
| `/avisos` | Consulta os avisos de um membro. |
| `/remover-aviso` | Remove um aviso pelo ID. |
| `/limpar-avisos` | Remove todos os avisos de um membro. |
| `/inspecionar` | Consulta o perfil de moderação de um membro. |
| `/nota` | Registra uma nota interna sobre um membro. |
| `/purge` | Apaga mensagens com filtros de autor, conteúdo ou bots. |
| `/lockdown` | Bloqueia ou desbloqueia um canal para membros comuns. |
| `/palavra-proibida` | Consulta ou edita a lista legada de palavras, sem ativar filtragem automática. |

As ações exigem as permissões correspondentes de quem as solicita e do próprio bot. Os avisos são registros: atingir uma quantidade de avisos não aplica mute, kick ou ban. Os filtros e as punições automáticas estão desativados no fluxo atual, mesmo que existam configurações antigas no banco.

### Utilidades

Painel de ajuda, informações do bot e utilidades por menção, incluindo avatar, informações de servidor, cargos e canais, enquetes, lembretes, cores, timestamps, resumo e tradução.

| Comando | Função |
| --- | --- |
| `/ajuda` | Abre o painel interativo de ajuda. |
| `/ping` | Mostra a latência e informações de saúde dos serviços. |
| `/botinfo` | Apresenta os recursos e as estatísticas do bot. |

As demais utilidades são solicitadas em mensagens, por exemplo: `@Revolutx avatar do @membro`, `@Revolutx info do servidor`, `@Revolutx traduz isso para inglês: [texto]` e `@Revolutx me lembra daqui 30 minutos de tomar água`. Use uma menção real à aplicação instalada; o nome exibido pode ser diferente.

## Adicionar ao servidor

A disponibilização do bot e o convite de instalação devem ser combinados com o mantenedor. Esta página não oferece um link público de convite nem exige que você forneça tokens ou chaves de API.

Para usar o Revolutx em um servidor onde ele já está instalado, siga as etapas abaixo.

## Primeira configuração

1. Execute `/ajuda` para abrir o painel de comandos.
2. Mencione o bot em uma mensagem para iniciar uma conversa.
3. Use `/perfil-ia` para escolher seu estilo de resposta e nível acadêmico.
4. Para estudar um tema, envie uma menção real ao bot seguida de `acadêmico iniciar [tema]`.
5. Use `/memoria-ia` para consultar e controlar suas memórias.

Administradores podem usar `/canal-ia` para ativar ou desativar respostas automáticas em um canal. Para configurar registros de moderação, use `/config-mod` com um canal de logs restrito à equipe.

## Permissões e privacidade

O bot precisa de acesso aos canais em que será usado e de permissão para enviar mensagens e apresentar links. As funções de moderação dependem das permissões correspondentes do bot e de quem solicita a ação, além da hierarquia dos cargos.

As respostas de IA dependem da disponibilidade dos serviços configurados pelo mantenedor. Mensagens, documentos e trechos de contexto podem ser enviados a provedores externos para gerar respostas.

Use `/limpar-conversa` para limpar o histórico de conversa e `/memoria-ia` para gerenciar as memórias. São controles distintos. Notas e registros de moderação são gerenciados pela equipe do servidor.

## Dúvidas e sugestões

Consulte `/ajuda` e procure a equipe do servidor se um comando não estiver disponível. Administradores podem usar `/status-ia` e `/testar-ia` para verificar os serviços.

Ao relatar um problema, informe o comando utilizado e o comportamento observado, sem publicar credenciais, documentos privados ou conversas de outros membros.
