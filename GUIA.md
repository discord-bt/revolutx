# Guia de uso

[Voltar à apresentação](README.md) · [Site oficial](https://revolutxbot.netlify.app/)

Os exemplos usam `@RevolutX` como menção ao bot. Selecione a aplicação na lista de menções do Discord; apenas digitar o nome como texto não a menciona. Substitua os trechos entre colchetes pelo conteúdo desejado.

## Comandos principais

| Comando | Uso |
| --- | --- |
| `/ajuda` | Abre o painel interativo de comandos. |
| `/botinfo` | Mostra a apresentação e informações do bot. |
| `/ping` | Consulta a latência e o estado dos serviços. |
| `/clima` | Consulta o clima de uma cidade. |
| `/perfil-ia` | Define seu estilo de resposta e nível acadêmico preferidos. |
| `/memoria-ia` | Consulta, registra ou apaga memórias e oferece controles do perfil e da conversa. |
| `/limpar-conversa` | Limpa seu histórico de conversa com o bot. |

## Pesquisa e tradução

```text
@RevolutX pesquisar: descobertas recentes sobre exoplanetas
@RevolutX acadêmico iniciar lógica proposicional
@RevolutX traduzir para inglês: A reunião começa às oito.
```

Para uma explicação comum, basta escrever sua pergunta. Para obter uma resposta mais extensa, peça aprofundamento. Pesquisa e referências dependem dos resultados encontrados; não há garantia de que toda consulta encontre fontes suficientes.

## Clima

Use `/clima` ou envie:

```text
@RevolutX clima Goiânia
```

O cartão apresenta as condições disponíveis para a localidade, com temperatura, sensação térmica e outros indicadores. O tema acompanha o dia ou a noite, e o horário exibido corresponde à localidade consultada. Dados indisponíveis não devem ser interpretados como zero. Se houver cidades homônimas, especifique melhor a localização.

## Imagens

| Pedido | Como usar |
| --- | --- |
| Criar | `@RevolutX criar imagem: um gato rosa e azul ciano` |
| Analisar | `@RevolutX analisar imagem: descreva esta imagem`, com anexo |
| Tons de cinza | `@RevolutX imagem cinza`, com anexo |
| Espelhar | `@RevolutX imagem espelhar`, com anexo |
| Girar | `@RevolutX imagem girar`, com anexo |
| Reduzir | `@RevolutX imagem reduzir`, com anexo |
| Editar por instrução | `@RevolutX editar imagem: deixe o céu azul`, com anexo, quando o serviço habilitado permitir |

A criação também aceita a forma sem dois-pontos: `@RevolutX criar imagem um gato rosa`. As edições simples não dependem de geração por IA. A criação, a análise e a edição generativa dependem das funções habilitadas e da disponibilidade dos serviços.

## Tarefas

```text
@RevolutX tarefa adicionar: revisar o capítulo de lógica
@RevolutX tarefas
@RevolutX tarefa concluir 12
```

Use o número retornado pelo bot no lugar de `12`. A lista pertence ao usuário no servidor, mas a resposta é publicada no canal da consulta. Para lembretes e outras utilidades, consulte `/ajuda`.

## Embeds e mensagens fixadas

Para preparar um embed, separe o título, a descrição e a cor com `|`:

```text
@RevolutX embed: Grupo de estudos | Encontro hoje às 20h. | #5865F2
```

A cor é opcional. O bot apresenta uma prévia; confirme para publicar ou cancele. A criação de embeds exige a permissão de gerenciar o servidor.

Para fixar ou desafixar, responda à mensagem desejada no mesmo canal:

```text
@RevolutX fixar
@RevolutX desfixar
```

Essas ações exigem a permissão de gerenciar mensagens, tanto de quem solicita quanto do bot.

## Personalização do servidor

Disponível para membros com permissão de gerenciar o servidor:

| Pedido | Efeito |
| --- | --- |
| `@RevolutX personalidade: responda de forma breve e acolhedora` | Ajusta o estilo do bot para a comunidade. |
| `@RevolutX nome bot: RevolutX Estudos` | Altera o apelido no servidor. |
| `@RevolutX foto bot anexo`, com imagem | Solicita a atualização da foto no servidor. |
| `@RevolutX foto bot remover` | Remove a foto personalizada do servidor. |
| `@RevolutX perfil bot ver` | Consulta a personalização de conversa. |
| `@RevolutX perfil bot resetar` | Restaura a personalidade e a preferência de modelo; não altera nome ou foto. |
| `@RevolutX chat automático ativar` | Ativa respostas automáticas no canal atual. |
| `@RevolutX chat automático desativar` | Desativa respostas automáticas no canal atual. |

Mudanças de nome e foto dependem das permissões e dos recursos disponíveis no Discord. A personalização do servidor é distinta do perfil pessoal configurado em `/perfil-ia`. Administradores também podem controlar os canais com `/canal-ia`.

## Moderação e administração

A moderação é manual. A equipe pode consultar e remover avisos, registrar notas, limpar mensagens e controlar canais com comandos como `/avisos`, `/remover-aviso`, `/limpar-avisos`, `/inspecionar`, `/nota`, `/purge` e `/lockdown`. Use `/config-mod` para configurar os registros.

Banimentos, expulsões e silenciamentos por menção exigem as permissões correspondentes e respeitam a hierarquia de cargos. Consulte os exemplos em `/ajuda` antes de executar uma ação.

Administradores dispõem de `/status-ia` e `/testar-ia` para consultar a disponibilidade da IA. Os comandos administrativos não ficam acessíveis a todos os membros.

## Quando um comando não funciona

Confira a menção, os argumentos e as permissões no canal. Em pedidos de imagem, verifique se o anexo foi enviado. Se uma função estiver indisponível, procure a equipe do servidor com o comando utilizado e a mensagem recebida. Não publique tokens, documentos privados ou dados de outros membros no relato.
