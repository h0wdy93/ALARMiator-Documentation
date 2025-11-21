---
title: "MP-FEUER ELS Plugin"
slug: /mpfeuerplugin
---

# MP-FEUER ELS Plugin

Dieses Plugin leitet die Daten eines eingehenden Alarm über die MP-Feuer ELS Schnittstelle weiter in MP-Feuer.

Vorraussetzungen in MP-Feuer:

- MP-Feuer Terminal Installation
- MP-Feuer ELS Plugin aktiviert und erreichbar
- Schnittstellenbenutzer mit der Berechtigung einen Alarm anzulegen


Einstellungen im Alarmiator-Plugin:

Plugin Aktiv Ja
Benutzername + Passwort des MP-Feuer Schnittstellen-Nutzer
HTTP oder HTTPS, je nach Einstellung des MP-Feuer Server.
Addresse der ELS Schnittstelle des MP-Feuer Server.
Port angeben (Standard ist 443)

Mapping der Gruppen:
Die im Alarmiator alarmierten Gruppen müssen hier zu der alarmierten Abteilung in MP-Feuer zugeordnet werden, auf Basis der IDs.
In MP-Feuer ist die ID der Abteilung die Abt-Nr., zu finden in Einstellungen -> Abteilungen.
Die Gruppen IDs in alarmiator sind über den Web-Browser zu finden. Stammdaten -> Gruppen. Dort eine Gruppe bearbeiten und in der URL ist hinter edit/ die ID der Gruppe zu finden. 

Um einen Alarm weiterzuleiten muss mindestens eine der alarmierten Gruppen mit der MP-Feuer Abteilung gemappt sein. Idealerweise gibt es eine Gruppe die immer alarmiert wird, z.B. für Einsatztablets. Dann reicht es diese eine Gruppe nur zu mappen und alle anderen können ignoriert werden. 

Nach Aktivierung des Plugins werden Alarme an den MP-Feuer Terminal-Server übertragen 