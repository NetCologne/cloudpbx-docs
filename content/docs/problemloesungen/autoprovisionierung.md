---
title: "Autoprovisionierung"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 602
toc: true
---

## MAC-Adressen
Es existieren unterschiedliche Schreibweisen der MAC-Adresse. Manche Hersteller schreiben sie zum Beispiel mit Doppelpunkten oder Strichen. **Wichtig**: Wenn Sie die MAC-Adresse in Ihrem Cloud PBX Konto angeben, lassen Sie Zeichen wie Punkte oder Striche weg.

Falls Sie bereits ein Telefon über die Weboberfläche für die Autoprovisionierung eingetragen haben und sich bei der MAC-Adresse vertippt haben, entfernen Sie bitte jenes zunächst aus der Weboberfläche. Tragen Sie es bitte danach mit der richtigen MAC-Adresse ein.

## Geraet meldet sich nicht beim NetCologne Provisioningserver
Ist dies der Fall können sie manuell den Provisioningserver direkt in der Benutzeroberfläche des Telefons eintragen:
Bei der **Yealink T4'er Serie** tragen sie unter "Setting -> Automatische Einrichtung -> Server URI" folgende URL ein: https://phones.cloudpbx.netcologne.de:1444/device/autoprov/config/\br
Bei der **Yealink T5'er Serie** tragen sie unter "Einstellungen -> Autoprovisioning -> Server URL" folgende URL ein: https://phones.cloudpbx.netcologne.de:1444/device/autoprov/config/\b
