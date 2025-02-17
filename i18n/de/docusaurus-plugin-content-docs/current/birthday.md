---
title: Geburtstage
description: TomatenKuchen ist ein All-in-One-Discord-Bot mit vielen verschiedenen Funktionen. Erklärt, wie man das Geburtstagssystem verwendet
---

Geburtstage werden täglich um 0 Uhr in der festgelegten Serverzeitzone geprüft.

## Reale Nutzer

### Geburtstag setzen/bearbeiten
Jeder Nutzer kann seinen Geburtstag global mithilfe von dem Befehl `birthday set <Tag> <Monat> [<Jahr>] [public]` festlegen.

Das Jahr ist optional, wenn angegeben ist bei Geburtstagsnachrichten und [automatisch updatenden Nachrichten](./autoupdate) der Parameter `{age}` verfügbar, womit das neue Alter angezeigt werden kann. Wenn das Jahr nicht angegeben wird ist der Alters-Parameter leer.

Mit der Option `public` wird festgelegt, ob der Geburtstag beim `user`-Befehl und beim `{birthday}`-Argument von Autoupdate-Nachrichten angezeigt wird. Geburtstagsankündigungen sind hiervon nicht betroffen.

- `birthday set 29 2 2000 public`
	- Legt einen öffentlichen Geburtstag fest, der jedes Jahr am 29.02. angekündigt wird. Wenn das Jahr kein Schaltjahr ist, so erscheint die Nachricht am 01.03.
- `birthday set 1 4`

### Geburtstag löschen
Solltest du deinen Geburtstag löschen wollen, verwende den Befehl `birthday delete`.

## Fiktive Geburtstage
Fiktive Geburtstage sind pro Server und können von Servermoderatoren erstellt und verwaltet werden.

### Erstellen/Bearbeiten
`birthday setfictive <Name> <Tag> <Monat> [<Jahr>]`
Fiktive Geburtstage müssen einen Namen haben, um sie identifizieren zu können. Mithilfe dieses Namens werden Geburtstagsnachrichten erstellt - die Argumente bleiben gleich und werden vom Bot automatisch angepasst - und `{birthday}` generiert.

- `birthday setfictive Minecraft 17 5 2009`
- `birthday setfictive 🎇Sylvester🎆 31 12`

### Löschen
`birthday deletefictive <Name>`

## Einstellungen

### Nachricht
Hier kann die Nachricht eingestellt werden, die gesendet wird, wenn ein realer oder fiktiver Nutzer Geburtstag hat.

### Kanal
Hier kann der Kanal festgelegt werden, in dem Geburtstage angekündigt werden.

### Rolle
Es kann eine Rolle ausgewählt werden, die Nutzer am Geburtstag für 24 Stunden erhalten.
