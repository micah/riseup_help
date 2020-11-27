@title = "Riseup чат"
@nav_title = "Чат"

## Что такое XMPP?

XMPP - это открытый стандарт для мгновенного обмена сообщениями. Поддерживает многопользовательские чаты, аудио и видеозвонки. With XMPP, you can send and receive messages between users on thousands of different chat providers.

## Использование Riseup's XMPP-сервиса

Ваш email адрес riseup.net также является вашим Адрес XMPP. For someone to send you an XMPP message or buddy request, they just need to send it to `username@riseup.net`.

Чтобы настроить [[XMPP-клиент => chat/clients]], вам необходима следующая информация:

- **протокол**: "xmpp"
- **аккаунт**: `username@riseup.net`
- **пароль**: ваш [[riseup-password]]

It is very important than you configure your client to **always require encryption**. Some clients have a setting "encryption if available". Even though the riseup.net servers require encryption, if your client is configured to use "encryption if available" an attacker can easily acquire your password.

Некоторые XMPP-клиенты могут запрашивать ваше имя пользователя и домен раздельно. В этом случае вы должны указать:

- **имя пользователя**: `username`
- **домен**: `riseup.net`

Учебные пособия по конкретным клиентам смотрите на странице [[XMPP-клиенты => chat/clients]].

## Подключение к многопользовательским чатам (конференциям, комнатам)

При подключении или создании конференции в XMPP-сети Riseup's, синтаксис должен быть следующим:

- `имя-вашей-комнаты@conference.riseup.net`

Если необходимо указать комнату отдельно, укажите следующее:

- **имя комнаты**: `имя-вашей-комнаты`
- **домен**: `conference.riseup.net`

НЕ используйте `имя-вашей-комнаты@riseup.net`

### Использование комнат в Pidgin

Если вы подключены через [[pidgin]], чтобы присоединиться или создать комнату, нажмите `Добавить чат` в меню `Собеседники`.

- **Комната**: `имя-комнаты`
- **Сервер**: `conference.riseup.net`
- **Имя**: `ваш-ник`
- **Пароль**: `необязательно`
- **Псевдоним**: `необязательно`
- **Группа**: `необязательно`

Нажмите `Добавить`. В списке собеседников вы должны увидеть группу с вашей комнатой.
Щелкните правой клавишей по комнате и нажмите `Присоединиться`.

Для тестирования, вы можете выбрать `riseup.net` в качестве названия комнаты и присоединиться к ней.

## Для дополнительной безопасности

1. Для дополнительной безопасности заходите на наш XMPP-сервер через [[Riseup VPN => vpn]].
1. Используйте наш ["Tor hidden service"](https://www.torproject.org/docs/hidden-services.html.en): адрес(`xmpp.*.onion`) которого вы можете найти на [[Riseup's onion services pages->tor#riseups-tor-hidden-services]].
