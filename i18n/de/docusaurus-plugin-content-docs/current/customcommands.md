---
title: Customcommands
description: TomatenKuchen ist ein All-in-One-Discord-Bot mit vielen verschiedenen Funktionen. Erklärt Customcommands und listet mögliche Parameter auf
---

:::caution

Customcommands sind veraltet und sollten nicht mehr verwendet werden. Sie wurden durch [Integrationen](/integrations) ersetzt - weitere Informationen findest du dort.

:::

Um Customcommands zu verwalten brauchst du die Berechtigung "Server verwalten".
Es wird empfohlen, dafür unser [Dashboard](https://tomatenkuchen.eu/dashboard/customcommands) zu nutzen.

## Befehle

### Erstellen

`customcommand <Name> <Inhalt>`

Beispiel:
`customcommand hi Hey ^^`

### Bearbeiten

`customcommand <Name> <Neuer Inhalt>`

Beispiel:
`customcommand hi Hallo!`

### Löschen

`customcommand <Name> del`

Beispiel:
`customcommand hi del`

### Raw-Code anzeigen

`customcommand <Name> raw`

Beispiel:
`customcommand hi raw`
-->
`Hallo!`

### Testen

`customcommand test <Customcommand-Code>`

Beispiel:
`customcommand test Hallo **{author.name}**! :D`

## Variablen

* Erwähnung: `{author}`
* Nutzer-ID: `{author.id}`
* Nickname: `{author.name}`
* Benutzername: `{author.username}`
* Discriminator: `{author.discrim}`
* Avatar: `{author.avatar}`
* Account erstellt: `{author.created}`
* Beigetreten: `{author.joined}`
* Servername: `{server.name}`
* Server-ID: `{server.id}`
* Server-Icon: `{server.icon}`
* Serverbesitzer: `{server.owner}`
* Nutzer auf dem Server: `{server.members}`
* Bots: `{server.members.bots}`
* Nutzer: `{server.members.humans}`
* Kanal-Erwähnung: `{channel}`
* Kanalname: `{channel.name}`
* Kanal-ID: `{channel.id}`
* Kanal-Thema: `{channel.topic}`
* Kanal-Kategorie: `{channel.category}`
* Kanal-Kategorie-ID: `{channel.category.id}`
* Prefix: `{prefix}`
* Unix-Timestamp: `{unix}`
* Unix-Timestamp in Sekunden: `{unixsec}`

* Alias für anderen Customcommand hinzufügen: `{alias:<Name>}`
* Rolle erzwingen: `{requirerole:<ID>}`

* Argumente: `{1} {2} {3} ... {args}`
* Argumente erzwingen: `{!1} {!2} {!3} ...`
* Bot-Befehl ausführen: `{run:<Befehl>}`
* JSON-API: `{jsonapi:<URL> <Property|RANDOM>}`
* Customcommand-Nachricht nicht löschen: `{nodel}`

**Embeds:**
* Embed aktivieren: `[embed]`
* Titel setzen: `[title:<Text>]`
* Beschreibung setzen: `[description:<Text>]`
* Bild setzen: `[image:<Bild-URL>]`
* Footer setzen: `[footer:<Text>]`
