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

Sie befinden sich nun in der Administrator-Maske der CloudPBX. Das Dashboard liefert eine Überischt zu Nachrichten (Messages), Anrufen (Calls), Faxeinstellungen, den registrierten Endgeräten und der ...

## PBX-Konfiguration

![cloudpbx konfiguration](https://user-images.githubusercontent.com/98753538/158146352-44ab0a62-5820-434c-b90d-a19b127380f2.jpg)

Gehen Sie bei der Einrichtung Ihrer Telefonanlage am besten wie folgt vor:

### 1. Seats = Nebenstellen <br>
Damit Sie telefonieren können, müssen Sie zunächst **Nebenstellen** einrichten. Erst ab dem Zeitpunkt der Einrichtung der Nebenstellen entstehen Kosten für die jeweilige Rufnummer. Hier finden Sie die Beschreibung, wie Sie eine [Nebenstelle einrichten](https://cloudpbx-doku.netcologne.de/docs/konfiguration/seats/) <br>
Es ist hilfreich, wenn Sie sich vorher den *Verwendungszweck* der Nebenstelle überlegen. Soll die Nummer einem *Telefon* zugewiesen werden oder handelt es sich um eine *Voice- oder Faxbox*? Oder soll hinter der Nummer ein Anrufmenü geschaltet werden? <br>
Mehrere Nebenstellen können in einer *Gruppe* zusammengefasst werden. Außerdem werden viele Sonderfunktionen wie *Anrufmenü, Faxserver oder Voiceboxen* über *Anrufweiterschaltungen* realisiert. Die *Anrufweiterschaltung* und damit die Aktivierung der entsprechenden Funktion kann durch den Besitzer der Nebenstelle oder durch den Administrator, dann aber über den Menüpunkt *"Kundendetails"*, aktiviert werden. <br>
Von allen diesen Überlegungen hängt dann die weiteren Konfiguration ab. <br> 

### 2. Gruppen <br>
Eine Sonderform der Nebenstelle ist eine **Gruppen**. Dabei werden ohne zusätzliche Kosten mehrere Nebenstellen zu einer solchen zusammengefasst. Hier können sie die Einstellungen für eine [Gruppennummer festlegen](https://cloudpbx-doku.netcologne.de/docs/konfiguration/gruppen/) <br>

### 3. Geräte <br>
Hier ist beschrieben, wie Sie die **Telefone** konfigurieren und den Nebenstellen zuweisen. Zuvor haben Sie sich die Struktur überlegt, welche Mitarbeiter zusammenarbeiten und welche Mitarbeiter den *Presence-Status* von welchen Kollegen erhalten sollen. Entsprechend können Sie dann z.B. *BusyLampFields* einrichten.
Yealink und SNOM Telefone können teilweise autoprovisioniert werden. Wie sie in diesen Fällen vorgehen, erfahren Sie hier: [Geräte einrichten](https://cloudpbx-doku.netcologne.de/docs/konfiguration/geraete/#einrichten-von-ger%C3%A4ten). <br>
Falls bei ihrem Gerät keine *Autoprovisionierung* möglich ist, schauen sie unter dem Menüpunkt *"Endgeräte"* nach, ob eine manuelle Provisionierungsanleitung vorhanden ist.   

### 4. Anrufwarteschlangen <br>
**Anrufwarteschlangen** sorgen dafür, dass auch bei besetzter Nebenstelle Anrufe nicht abgewiesen und stattdessen in eine Warteschlange eingereiht werden.
Der Anrufer erhält eine Begrüssungsansage und eine Information, an welcher Stelle der Warteschlange er sich befindet. Details zur Konfiguration finden Sie unter [Anrufwarteschlangen einrichten](https://cloudpbx-doku.netcologne.de/docs/konfiguration/anrufwarteschlangen-einrichten/) <br>

### 5. SoundSets <br>
Die **Soundsets** sind vorkonfiguriert, müssen aber entsprechend Ihren Anforderungen angepasst werden. Dies gilt insbesondere für die Ansagen des Anrufmenüs. Sie können hier aber auch die *Wartemusik* anpassen oder *"OutOfOffice" Ansagen* definieren. Wie Sie bei der Konfiguration vorgehen ist, steht hier: [Soundsets](https://cloudpbx-doku.netcologne.de/docs/konfiguration/sound-sets/) <br>
Achtung: Individuelle Ansagen für die Voicebox werden hier nicht bereitgestellt. Diese sollen durch den Besitzer der Nebenstelle definiert werden. Dazu ist der Loging auf dem direkten Nebenstellenaccount erforderlich. Alternativ kann der Administrator diese Einstellungen auch über den Menüpunkt "Kundendetails" vornehmen. 

### 6. Geschäftsführungssekretariat <br>
[Sekretariat einrichten](https://cloudpbx-doku.netcologne.de/docs/konfiguration/sekretariat-einrichten/) <br>

### 7. Anrufmenü (AutoAttendant) <br>
Hier können Sie ein bis zu 10-stufiges **Anrufmenü** konfigurieren. Sie legen die Ziele fest, die den einzelnen Auswahlpunkten entsprechen sollen. Ziele können *Gruppen, Nebenstellen, Voiceboxen, Mobilnummern* oder auch weitere *Anrufmenüs* sein. Wie Sie bei der Konfiguration vorgehen, ist hier beschrieben: [Anrufmenü](https://cloudpbx-doku.netcologne.de/docs/konfiguration/anrufmenue/) <br>
