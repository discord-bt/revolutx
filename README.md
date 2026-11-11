# RevolutX

Assistente de inteligência artificial para Discord, com conversa contextual, apoio aos estudos, pesquisa, clima e ferramentas para comunidades.

[Site oficial](https://revolutxbot.netlify.app/) · [Adicionar ao Discord](https://discord.com/oauth2/authorize?client_id=1487512494674153793&permissions=8&integration_type=0&scope=bot%20applications.commands) · [Guia de comandos](GUIA.md)

## Começar

Adicione o RevolutX pelo convite oficial, escolha o servidor e revise as permissões solicitadas pelo Discord. O convite atual solicita a permissão Administrador. Depois da instalação, abra `/ajuda` e mencione o bot para conversar.

```text
@RevolutX oi
@RevolutX explique resumidamente o que é uma contradição lógica
```

Use uma menção real ao bot. Não é necessário baixar arquivos, hospedar uma cópia ou fornecer uma chave de API para usá-lo no servidor.

## Recursos

| Recurso | O que você pode fazer |
| --- | --- |
| Conversa | Conversar por menção ou responder a uma mensagem do bot, usando o contexto da conversa. |
| Estudo e pesquisa | Pedir explicações, aprofundar um assunto e consultar fontes para pesquisas e informações atuais. |
| Perfil e memória | Escolher o estilo de resposta, gerenciar memórias e limpar o histórico de conversa. |
| Clima | Consultar uma cidade em um cartão com aparência de dia ou noite e horário local. |
| Imagens | Analisar anexos, criar imagens por descrição e aplicar edições simples. |
| Organização | Criar tarefas pessoais por servidor, consultar pendências e marcar conclusões. |
| Mensagens | Preparar embeds com prévia e confirmação, além de fixar ou desafixar mensagens. |
| Personalização | Ajustar personalidade, nome e foto do bot no servidor, conforme permissões e disponibilidade. |
| Utilidades | Traduzir textos, usar lembretes, consultar avatares e informações do servidor. |
| Moderação | Executar ações manuais e gerenciar avisos, notas e limpeza de mensagens. |

Os recursos de IA e pesquisa dependem dos serviços disponíveis. A edição de anexos por instruções depende do serviço de imagem habilitado; criar uma imagem nova e editar uma existente são funções distintas.

## Conversa e estudo

As respostas procuram acompanhar o tom e o assunto da conversa. Uma pergunta simples pode receber uma explicação breve; peça “explique melhor” ou “aprofunde” quando quiser mais detalhes. O registro acadêmico é usado quando o pedido exige maior rigor, sem transformar toda conversa em uma análise extensa.

O apoio aos estudos abrange lógica, matemática, filosofia, história, política, teologia, biologia, física e química. Para iniciar uma sessão de estudo, envie `@RevolutX acadêmico iniciar [tema]`. Para pedir uma consulta externa, use `@RevolutX pesquisar: [assunto]`.

As pesquisas apresentam fontes quando elas são recuperadas. Confira as referências antes de utilizá-las em trabalhos; uma resposta do bot não substitui a leitura do material original.

## Para a administração

A equipe pode configurar os canais de conversa automática, personalizar o bot e usar ferramentas de organização e moderação. As ações respeitam as permissões necessárias e a hierarquia de cargos.

Os avisos são registros de moderação: acumular avisos não aplica automaticamente mute, kick ou ban.

Consulte o [guia de comandos](GUIA.md) para exemplos de uso e diferenças entre recursos pessoais e administrativos. O painel `/ajuda` reúne os comandos disponíveis na instalação.

## Dados e privacidade

Mensagens, anexos e trechos de contexto usados nas funções de IA podem ser enviados a serviços externos para produzir respostas. Evite enviar informações confidenciais. Tarefas e respostas podem aparecer no canal em que são solicitadas.

Use `/limpar-conversa` para limpar seu histórico de conversa e `/memoria-ia` para gerenciar as memórias. São controles distintos. Registros de moderação são administrados pela equipe do servidor.

## Sobre este repositório

Este é o guia público do RevolutX, mantido por [pyyrho](https://github.com/pyyrho). Ele apresenta funcionalidades e orientações de uso. O código-fonte do bot é privado; este repositório não distribui plugins instaláveis nem uma versão para hospedagem própria.

Para dúvidas, consulte `/ajuda` e a equipe do servidor. Ao relatar um problema, informe o comando e o resultado observado, sem publicar credenciais ou conversas privadas.

Documentação atualizada em 11 de novembro de 2026.
