@title = "Segurança de bate-papo"

## Proteja suas mensagens

Na maioria dos casos, quando você usar o serviço de XMPP do Riseup, as suas mensagens serão criptografadas em trânsito. Não existe, porém, garantia disso, a não ser que ambas as partes usem Riseup.

Para assegurar a criptografia ponta a ponta das mensagens, a melhor opção é o protocolo [[Off-the-Record (ORT) -> https://en.wikipedia.org/wiki/Off-the-Record_Messaging]]. Para mais informações, leia nosso [[tutorial sobre OTR -> otr]].

## Chamadas seguras

Da última vez que checamos, Jitsi era o único cliente de XMPP que oferecia ligações de voz e vídeo seguras.

## Use IRC com segurança

- **SSL** - Veja [[security/network-security/certificates]]. Para acessar o canal do #riseup hospedado na rede IndyMedia, use a porta 6697.
- **Autenticação externa com SASL** e **impressão digital de certificado (CertFP)** - Mecanismos diferentes, mas relacionados, de autenticação por meio de certificados. Usados juntos, possibilitam que você se autentique em um serviço antes que a conexão de rede esteja completa e sem precisar de senha.
  * Registre seu nick: `/msg nickserv register <senha> <e-mail>`.
  * Crie seu certificado: `openssl req -x509 -new -newkey rsa:4096 -sha256 -days 1000 -nodes -out riseup.pem -keyout riseup.pem`.
  * Ajuste o cliente para se conectar ao certificado via autenticação externa com SASL: [[exemplos no site da OFTC -> https://www.oftc.net/NickServ/CertFP/]].
  * Conecte-se usando o certificado.
  * Verifique se sua impressão digital com `/whois <seu-nick>` é igual à impressão digital do seu certificado. Acesse [[security/network-security/certificates]] para saber mais.
  * Adicione a impressão digital do certificado (CertFP): `/msg nickserv cert add`.
  * Guarde o certificado em local seguro, como se fosse uma senha.
