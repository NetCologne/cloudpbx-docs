---
title: "Rufgruppen"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "funktionen"
weight: 403
toc: true
---

Mit Rufgruppen kann der Administrator des NetCologne Cloud PBX Kontos eine gemeinsame Rufnummer für verschiedene Geräte vergeben. 


## Hunting-Regeln
Wenn Sie eine Gruppe anrufen, klingeln die Telefone der Mitglieder dieser Gruppe gemäß der gewählten Hunting-Regel.

### Serielles Klingeln
Serielles Klingeln bewirkt, dass es bei jedem Teilnehmer der Gruppe nacheinander für die gewählte Klingeldauer klingelt. Für die Reihenfolge ist es entscheidend, in welcher Reihenfolge die Teilnehmer der Gruppe hinzugefügt wurden. Hat es bei allen Teilnehmer der Gruppe nacheinander geklingelt, wird der Anruf abgewiesen.

### Paralleles Klingeln
Paralleles Klingeln bewirkt, dass es bei allen Teilnehmern in der Gruppe gleichzeitig klingelt. Dabei klingelt es solange, bis einer der Teilnehmern den Anruf annimmt.

### Zufälliges Klingeln
Zufälliges Klingeln ist wie serielles Klingeln nur mit zufälliger Reihenfolge.

### Zirkuläres Klingeln
Zirkuläres Klingeln bewirkt, dass es bei dem Teilnehmer klingelt, der nach dem Teilnehmer aufgeführt ist, der den letzten Anruf für diese Gruppe angenommen hat. Schlägt der erste Zustellungsversuch fehl, geht es sequentiell weiter.
