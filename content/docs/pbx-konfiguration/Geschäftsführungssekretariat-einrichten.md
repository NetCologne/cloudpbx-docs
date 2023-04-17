---
title: "Geschäftsführungssekretariat einrichten"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 207
toc: true
---

Die Cloud-PBX-Funktion **Geschäftsführungssekretariat** bietet die Möglichkeit Anrufe zur Geschäftsführung (Chef/Chefin) gezielt zu steuern. Sämtliche Anrufe zur  Durchwahl des/der Vorgesetzten, werden zunächst zu einem Mitarbeiter (Sekretär/in) weitergeleitet und dort entgegengenommen. Je nachdem, ob Gespräche gewünscht sind, können Anrufe dann zum Vorgesetzten druchgestellt oder ggf. direkt vom Mitarbeiter (Sekretär/in) beantwortet werden.

## 1. Grundkonfig einrichten 

Im Beispiel ist *porz* der Geschäftsführer. Das *Sekretariat* hat die Rufnummer 492212615245417. In der PBX-Konfiguration den Menuepunkt **Geschäftsführungssekretariat** anklicken, dann den Manager (hier: porz) auswählen.

![GF-Sekretärin einrichten](https://user-images.githubusercontent.com/98753538/232427318-0c806532-a1e5-46ea-9d12-82b016094988.jpg)

Nun diesem die Rufnummer des Mitarbeiters (Sekretär/in) zuweisen und die Konfiguration bestätigen.

![GF-Sekretärin hinzufügen](https://user-images.githubusercontent.com/98753538/232438884-e6149b06-112e-4c77-b6b8-e1d0c56ebda6.jpg)

## 2. Konfiguration durch Weiterleitung aktivieren

Damit die Konfiguration funktioniert, muss nun noch für den Subscriber *porz* eine *Weiterleitung zur Sekretärin* eingerichtet werden. 
Dafür unter Kundendetails den subscriber *porz* auswählen.

![GF-Sekretärin subscriber](https://user-images.githubusercontent.com/98753538/232429453-48e80161-50b0-4b63-840e-f8cfebc57ea5.jpg)

Beim betreffenden Subscriber rechts auf den Punkt *Einstellungen* klicken und dann im Menuepunkt *Call Forwards* die Weiterleitung zu **Manager Secretary** einrichten.

![GF-Sekretärin weiterleiten](https://user-images.githubusercontent.com/98753538/232430441-8acbebae-441b-40a9-8272-5d2ac3c85fca.jpg)

Mit dem Klick auf *Save* werden die Einstellungen gespeichert und aktiviert.
