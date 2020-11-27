@title = "Bate-papo Riseup"
@nav_title = "Bate-papo"

## O que é XMPP?

XMPP é um padrão aberto para troca de mensagens instantâneas que também abrange conversas de voz e vídeo. Com XMPP, você pode trocar mensagens com usuários de milhares de diferentes provedores de bate-papo.

## Usando o XMPP de Riseup

Seu endereço de e-mail riseup.net serve também como endereço de XMPP. Para alguém lhe enviar uma mensagem XMPP ou solicitação de amizade, é necessário apenas endereçá-la a `nome-de-usuario@riseup.net`.

Para configurar um [[cliente de XMPP => chat/clients]], você precisa destas informações:

- **Protocolo**: "xmpp".
- **Conta**: `nome-de-usuario@riseup.net@`
- **Senha**: sua [[senha Riseup => riseup-password]].

É de extrema importância que você configure seu cliente para **sempre requerer criptografia**. Alguns clients têm a opção "criptografia, se disponível". Mesmo que os servidores riseup.net exijam criptografia, se o seu cliente for configurado para usar "criptografia, se disponível", um hacker pode facilmente descobrir sua senha.

Alguns clientes de XMPP pedem nome de usuário e domínio separadamente. Neste caso, você deve especificar:

- **Nome de usuário**: `nome-de-usuario`.
- **Domínio**: `riseup.net`.

Para tutoriais de clientes específicos, veja nossa página sobre [[clientes de XMPP => chat/clients]].

## Conectando-se a salas de bate-papo multiusuário

Quando criar ou se conectar a uma sala de bate-papo na rede XMPP de Riseup, refira-se a ela nesta sintaxe:

- `nome-da-sua-sala@conference.riseup.net`

Se precisar especificar a sala separadamente, faça o seguinte:

- Sala de bate-papo: `nome-da-sua-sala`.
- Domínio: `conference.riseup.net`.

*Não* assim:

- `nome-da-sua-sala@riseup.net`

### Usando salas no cliente Pidgin

Se você se conectou via [[pidgin]] para criar ou entrar em uma sala de bate-papo, clique em `Adicionar bate-papo...` no menu `Amigos`.

- Sala: `nome-da-sua-sala`.
- Servidor: `conference.riseup.net`.
- Apelido: `seu-apelido`.
- Senha: [opcional].
- Alias: [opcional].
- Grupo: [opcional].

Clique em `Adicionar` e dê uma olhada na lista de amigos. Você deve notar um grupo `Bate-papos` com a sua sala.
Clique nele com o botão direito do mouse e selecione a opção `Entrar`.

Para testes, você pode nomear a sala como `riseup.net` e nela entrar.

## Para segurança adicional

1. Para segurança adicional, acesse nosso servidor de XMPP através da [[VPN Riseup => vpn]].
1. Use o ["serviço oculto de Tor"](https://www.torproject.org/docs/hidden-services.html.en) procure por `xmpp.*.onion` na página sobre [[os serviços de onion do Riseup -> tor#riseups-tor-hidden-services]].
