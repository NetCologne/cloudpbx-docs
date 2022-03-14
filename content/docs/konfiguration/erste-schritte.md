---
title: "Erste Schritte"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "konfiguration"
weight: 201
toc: true
---

Nun machen Sie sich mit Ihrer NetCologne Cloud PBX vertraut. In diesem Abschnitt erfahren Sie, wie Sie am besten bei der Konfiguration Ihrer Anlage vorgehen.

## Anmeldevorgang

Die Anmeldung erfolgt über folgende Punkte:

Via E-Mail haben Sie die Zugangsdaten zu Ihrem NetCologne Cloud PBX Konto bekommen. Dieses Konto ist immer das Administrator-Konto. 

Webseite: [https://myportal.cloudpbx.netcologne.de/v2](https://myportal.cloudpbx.netcologne.de/v2/ "Cloud-PBX Konfiguration")   
Benutzer: `+49ONKZRufNr@firma.cloudpbx.netcologne.de`  
Passwort: `xxxxxxxxxxxxxx`  

Auf der angebenen Seite können Sie sich mit diesen Daten anmelden

![cloudpbx_login](https://user-images.githubusercontent.com/98753538/152331121-be008d22-e8da-4997-88f2-47daf5f423f7.jpg)

Sie befinden sich nun in der Administrator-Maske der CloudPBX. Das Dashboard liefert eine Überischt zu Nachrichten (Messages), Anrufen (Calls), der Konfiguration und den registrierten Endgeräten.

![cloudpbx_dashboard](https://user-images.githubusercontent.com/98753538/158141158-8a1401a7-f9a3-42c3-ac3f-9baebe6e3210.jpg)

Gehen Sie bei der Einrichtung Ihrer Telefonanlage am besten wie folgt vor:

1. Nebenstellen (Seats) einrichten: Damit Sie telefonieren können, müssen Sie zunächst Nebenstellen einrichten. Erst ab dem Zeitpunkt der Einrichtung der Nebenstellen entstehen Kosten für die jeweilige Rufnummer.
Wie Sie bei der Einrichtung der Nebenstellen vorgehen, ist hier (https://cloudpbx-doku.netcologne.de/docs/konfiguration/seats/) beschrieben.
Vorteilhaft ist es, wenn Sie sich zunächst den Verwendungszweck der Nebenstelle überlegen. Soll die Nummer einem Telefon zugewiesen werden oder handelt es sich um eine Voice- oder Faxbox? Oder soll hinter der Nummer ein Anrufmenü geschaltet werden? <br>
Hinweis: Viele Sonderfunktionen wie Anrufmenü, Faxserver oder Voiceboxen, werden über Anrufweiterschaltungen realisiert. Die Anrufweiterschaltungen und damit die Aktivierung der entsprechenden Funktion, können durch den Besitzer der Nebenstelle oder durch den Administrator, dann aber über "Kundendetails" aktiviert werden. Eine Sonderform der Nebenstelle ist eine Gruppennummer. Hinter Gruppennummern können mehrere Nebenstellen zusammengefasst werden. Dafür entstehen keine zusätzlichen Kosten. <br>
Von all diesen Überlegungen hängt dann die weiteren Konfiguration ab. 

2. Gruppen einrichten
Hier (Link) können sie die Einstellungen für eine Gruppennummer festlegen

3. Telefone konfigurieren und Nebenstellen zuweisen
Hier können Sie die Telefone einrichten und konfigurieren. Zuvor haben Sie sich die Struktur überlegt, welche Mitarbeiter zusammenarbeiten und welche Mitarbeiter den Presence-Status von welchen Kollegen erhalten sollen. Entsprechend können Sie dann z.B. BusyLampFields einrichten.
Yealink und SNOM Telefone können teilweise autoprovisioniert werden. Wie sie in diesen Fällen vorgehen ist hier (Link) beschrieben. Falls bei ihrem Gerät keine Autoprovisionierung möglich ist, schauen sie hier (Link) nach, ob eine manuelle Provisionierungsanleitung vorhanden ist.   

![cloudpbx_konfiguration](https://user-images.githubusercontent.com/98753538/158144030-bb298ac8-0daa-48fc-a049-1be97796390e.jpg)

4. Anrufwarteschlangen einrichten
Anrufwarteschlangen sorgen dafür, dass, auch bei besetzter Nebenstelle keine Anrufe abgewiesen und stattdessen in eine Warteschlange eingereiht werden.
Der Anrufer erhält eine Begrüssungsansage und eine Information, an welcher Stelle der Warteschlange er sich befindet. Ansagen und Wartemusik sind konfigurierbar (Link).
Wie sie bei der Einrichtung der Wartemusik vorgehen, ist hier (Link) beschrieben.

5. SoundSets konfigurieren
Die Soundsets sind vorkonfiguriert, müssen aber entsprechend Ihren Anforderungen angepasst werden. Dies gilt insbesondere für die Ansagen des Anrufmenüs. Sie können hier aber auch die Wartemusik anpassen oder "OutOfOffice" Ansagen definieren. Wie Sie bei der Konfiguration der SoundSets vorgehen ist hier (Link) beschrieben.
Achtung: Individuelle Ansagen für die Voicebox werden nicht hier definiert. Diese sollen durch den Besitzer der Nebenstelle definiert werden. Dazu ist der Loging auf dem direkten Nebenstellenaccount erforderlich. Alternativ kann der Administrator diese Einstellungen auch über "Kundendetails" vornehmen. 

6. Geschäftsführungssekretariat

7. Ein Anrufmenü (AutoAttendant) konfigurieren
Hier können Sie ein bis zu 10-stufiges Anrufmenü konfigurieren. Sie legen die Ziele fest, die den einzelnen Auswahlpunkten entsprechen sollen. Ziele können Gruppen, Nebenstellen, Voiceboxen, Mobilnummern oder auch weitere Anrufmenüs sein. Vorraussetzung für eine sinnvolle Nutzung ist die Konfiguration der SoundSets unter (Link).
Wie Sie bei der Konfiguration des Anrufmenüs vorgehen ist hier (Link) beschrieben
